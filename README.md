# rushilswork.github.io

> Personal portfolio — [rushilswork.github.io](https://rushilswork.github.io)

## About

Portfolio of **Rushil Pillamari**, Software Engineer based in Hyderabad, India. Built from scratch as a single-file static site — no frameworks, no build tools, no dependencies. 95KB total.

## Stack

- Vanilla HTML / CSS / JS — zero dependencies
- Playfair Display · Syne · JetBrains Mono (Google Fonts)
- CSS Scroll Timeline API (progress bar, native)
- CSS `clip-path` wipe (theme transition)
- CSS `perspective` + `transform-style: preserve-3d` (card flip)
- Canvas API (particle system + cursor trail)
- IntersectionObserver (scroll reveal)
- CSS custom properties (light/dark theming)
- Device Motion API (shake detection, iOS 13+ permission handled)

---

## Features

### Design
- Preloader with animated R mark and progress bar
- Character-by-character hero name reveal (post-preloader)
- Scroll-driven gold progress bar (CSS-native + JS fallback for Safari)
- Film grain overlay — oversized to prevent edge glitch
- Ghost section numbers 01–04 (clipped to section, hidden on mobile)
- Active nav highlight on scroll
- Back to top button
- Light / Dark mode — cinematic diagonal wipe transition (clip-path sweep)
- Theme preference persisted via `localStorage`

### Desktop-only
- Custom cursor with contextual labels and glow bloom
- Hero orb parallax (mouse-driven)
- Magnetic contact buttons
- Hold `Shift` + move mouse → gold constellation cursor trail
- Backtick `` ` `` → full-screen terminal

### Mobile-only
- Hamburger nav menu with fullscreen overlay
- Shake device → dust dissolve effect (iOS 13+ permission auto-requested)
- Long-press anywhere 800ms → full-screen terminal
- Terminal keyboard-aware: `100dvh` shrinks to visible area above keyboard
- Body scroll fully locked when terminal open, position restored on close

### Both devices
- Scroll reveal animations — skew, blur, slide, rise per element
- Skill tag stagger on reveal
- Stat counter animation on scroll into view
- 3D card flip on single click / tap — all 3 project cards
- Triple-click → all headings dissolve into gold dust and reform

---

## Hidden Features

### Desktop

| Trigger | Effect |
|---|---|
| Triple-click anywhere | All headings dissolve into gold dust, then reform |
| Type `rushil` | Hero name crumbles and rebuilds |
| Type `hireme` | Gold sparks fly to contact + `✦ Let's talk` toast + scroll |
| Idle 25 seconds | Particles crumble in from all four screen edges |
| Backtick `` ` `` | Full-screen terminal |
| Hold `Shift` + move mouse | Gold constellation cursor trail |
| Click any project card | Card flips in 3D revealing "behind the build" |

### Mobile

| Trigger | Effect |
|---|---|
| Triple-tap anywhere | All headings dissolve into gold dust, then reform |
| Shake device | Same dust dissolve effect |
| Long-press 800ms | Full-screen terminal (keyboard-aware, scroll-locked) |
| Tap any project card | Card flips in 3D revealing "behind the build" |
| Idle 25 seconds | Particles crumble in from all four screen edges |

### Terminal Commands
```
whoami · skills · projects · experience · contact · awards · hire rushil · clear · exit
```

---

## Sections

| # | Section |
|---|---|
| 01 | Hero |
| 02 | About + Stats |
| 03 | Skills |
| 04 | Work Experience |
| 05 | Projects — jobBot, Air Pollution Viz, Bandwidth Speed Test |
| 06 | Awards & Recognition |
| 07 | Contact |

---

## Local Development

No build step. Just open `index.html` in a browser.

```bash
# Or serve locally
npx serve .
# Visit http://localhost:3000
```

## Deployment

Hosted on **GitHub Pages** — auto-deploys on push to `main`.

```bash
git add index.html README.md
git commit -m "update"
git push
```

Live at: **https://rushilswork.github.io**

---

## License

MIT — feel free to use as inspiration. Please don't copy directly.

---

*Built with care. Designed to be fast, accessible, and memorable.*