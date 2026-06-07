# rushilswork.github.io

> Personal portfolio — [rushilswork.github.io](https://rushilswork.github.io)

## About

Portfolio of **Rushil Pillamari**, Software Engineer based in Hyderabad, India. Single-file static site — no frameworks, no build tools, no dependencies. 94KB.

## Stack

- Vanilla HTML / CSS / JS — zero dependencies
- Playfair Display · Syne · JetBrains Mono (Google Fonts)
- CSS Scroll Timeline API (progress bar, native + Safari fallback)
- CSS `clip-path` wipe (theme transition)
- CSS `perspective` + `transform-style: preserve-3d` (card flip)
- Canvas API (particle system + cursor trail)
- IntersectionObserver (scroll reveal + stat counters)
- CSS custom properties (light/dark theming)
- Device Motion API (shake, iOS 13+ permission auto-requested)

---

## Features

### Design
- Preloader — animated R mark + progress bar
- Character-by-character hero name reveal
- Scroll-driven gold progress bar (CSS-native, JS fallback for Safari)
- Film grain overlay — oversized `−10px` on all sides to prevent edge glitch
- Ghost section numbers 01–04 — clipped inside section, hidden on mobile
- Active nav highlight on scroll
- Back to top button (appears after 600px)
- Light / Dark mode — cinematic diagonal `clip-path` wipe (1.1s sweep in + out)
- Theme preference persisted via `localStorage`

### Animations
- Per-element scroll reveal — skew, blur, slide, rise (varied per element type)
- Skill tag stagger on reveal
- Stat counters animate up on scroll into view
- Section label line draws in
- Hero orb parallax on mouse move (desktop)
- Magnetic contact buttons (desktop)
- Gold glow sweep line on project card hover
- 3D card flip — single click/tap, all 3 cards, links inside exempt

### Responsive
- 4 breakpoints: `480px` / `768px` / `1024px` / `1400px`
- `100svh` hero with iOS browser chrome fix
- Touch device: native cursor, shake detection
- `prefers-reduced-motion` respected

---

## Hidden Features

### Desktop

| Trigger | Effect |
|---|---|
| Triple-click anywhere | All headings dissolve into gold dust, reform |
| Type `rushil` | Hero name crumbles and rebuilds |
| Type `hireme` | Gold sparks fly to contact + `✦ Let's talk` toast |
| Idle 25 seconds | Particles crumble in from all four edges |
| Backtick `` ` `` | Full-screen terminal |
| Hold `Shift` + move mouse | Gold constellation cursor trail |
| Click any project card | 3D flip revealing "behind the build" |

### Mobile

| Trigger | Effect |
|---|---|
| Triple-tap anywhere | All headings dissolve into gold dust, reform |
| Shake device | Same dust dissolve (iOS 13+ permission auto-requested) |
| Long-press 800ms | Full-screen terminal |
| Tap any project card | 3D flip revealing "behind the build" |
| Idle 25 seconds | Particles crumble in from all four edges |

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

No build step — open `index.html` directly in any browser.

```bash
# Or serve locally with live reload
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

MIT — use as inspiration, please don't copy directly.

---

*Built with care. Designed to be fast, accessible, and memorable.*