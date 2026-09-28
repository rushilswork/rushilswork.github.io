# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Personal portfolio site for Rushil Pillamari, deployed at rushilswork.github.io. It is a **single self-contained `index.html`** file (~100KB) with no build tools, no package manager, and no dependencies — all CSS is in one `<style>` block and all JS is in one `<script>` block at the end of the file, both inline in `index.html`. Fonts (Playfair Display, Syne, JetBrains Mono) load from Google Fonts via CDN link.

## Development

There is no build/lint/test tooling in this repo — edit `index.html` directly and view it in a browser.

```bash
# Preview locally
npx serve .
# or just open index.html directly in a browser
```

Deployment is GitHub Pages auto-deploy on push to `main`:

```bash
git add index.html README.md
git commit -m "update"
git push
```

## Architecture

`index.html` is organized as one long document with clearly HTML-commented section markers (`<!-- HERO -->`, `<!-- SKILLS -->`, `<!-- PROJECTS -->`, `<!-- TERMINAL -->`, etc.) — use these comments to jump to a section rather than searching blind. The page sections in DOM order are: nav → hero → marquee → about → skills → experience → projects → awards → contact → footer, plus several overlay elements defined before the nav (preloader, scroll progress bar, back-to-top, custom cursor, mobile menu, trail canvas, terminal overlay).

Key JS subsystems in the trailing `<script>` block (all vanilla, no modules/imports):
- **Theme system** — dark/light mode toggled via `data-theme` attribute on `<html>`, persisted to `localStorage` under key `rp-theme`, transitions with a `clip-path` diagonal wipe overlay.
- **Scroll effects** — `IntersectionObserver`-driven reveal animations, scroll-linked progress bar, active-nav-link highlighting, and animated stat counters, all keyed off section/element position.
- **Particle system** — a single `<canvas>` (`trailCanvas`/particle loop via `requestAnimationFrame`) shared by multiple effects: cursor trail (on `Shift`+mousemove), the heading "dust dissolve/reform" effect, and the 25-second idle-crumble animation.
- **Easter eggs / hidden interactions** — triple-click/triple-tap dust dissolve, typing `rushil` or `hireme` (keydown buffer matching), device-shake detection via `devicemotion`, and a full-screen terminal opened with backtick or long-press.
- **Terminal emulator** — `COMMANDS` object maps command names (`whoami`, `skills`, `projects`, `experience`, `contact`, `awards`, `hire rushil`, `clear`, `exit`) to output-generating functions; `termRun`/`termPrint` handle input parsing and rendering into the overlay.
- **Project cards** — 3D flip-on-click implemented with CSS `perspective`/`transform-style: preserve-3d`, toggled via a JS click handler per `.project-card-inner`.

When editing, keep new interactive behavior consistent with the existing patterns above (e.g., reuse the particle/canvas system for new visual effects rather than introducing a second canvas or animation loop).
