# rushilswork.github.io

> Personal portfolio — [rushilswork.github.io](https://rushilswork.github.io)

## About

Portfolio of **Rushil Pillamari**, Software Engineer based in Hyderabad, India. Built from scratch as a single-file static site — no frameworks, no build tools, no dependencies. 91KB total.

## Stack

- Vanilla HTML / CSS / JS — zero dependencies
- Playfair Display · Syne · JetBrains Mono (Google Fonts)
- CSS Scroll Timeline API (progress bar, native)
- CSS `clip-path` wipe (theme transition)
- CSS `perspective` + `transform-style: preserve-3d` (card flip)
- Canvas API (particle system + cursor trail)
- IntersectionObserver (scroll reveal)
- CSS custom properties (light/dark theming)
- Device Motion API (shake detection)

---

## Features

### Design
- Preloader with animated R mark and progress bar
- Character-by-character hero name reveal (post-preloader)
- Custom cursor with contextual labels and glow bloom
- Scroll-driven gold progress bar (CSS-native + JS fallback for Safari)
- Film grain overlay (animated)
- Ghost section numbers (01–04, clipped, hidden on mobile)
- Active nav highlight on scroll
- Back to top button (appears after 600px scroll)
- Hamburger mobile menu with fullscreen overlay

### Animations
- Per-element scroll reveal — varied per type (skew, blur, slide, rise, alternating)
- Skill tag stagger on reveal
- Stat counter animation (counts up on scroll into view)
- Section label line draws in on reveal
- Hero orb parallax (mouse-driven, desktop)
- Magnetic contact buttons (desktop)
- Slow-draw gold glow line on project card hover
- 3D card flip on double-click / double-tap

### Theme
- Light / Dark mode toggle
- Cinematic diagonal wipe transition between themes (1.1s clip-path sweep)
- All colors transition smoothly (0.3s) behind the wipe
- Preference persisted via `localStorage`

### Responsive
- 4 breakpoints: `480px` / `768px` / `1024px` / `1400px`
- Mobile hamburger menu, ghost numbers hidden, terminal hidden
- Touch device optimisations — native cursor, no custom cursor
- `prefers-reduced-motion` respected
- `100svh` hero with iOS browser chrome fix

---

## Hidden Features

| Trigger | Effect |
|---|---|
| Triple-click anywhere | All headings dissolve into gold dust particles, then reform |
| Shake device (mobile) | Same dust dissolve effect |
| Type `rushil` | Hero name crumbles into particles and rebuilds |
| Type `hireme` | Gold sparks fly to contact + `✦ Let's talk` toast + scroll |
| Idle 25 seconds | Particles crumble in from all four screen edges |
| Backtick `` ` `` (desktop) | Full-screen terminal — type `help` for commands |
| Double-click project cards | Cards flip in 3D revealing "behind the build" notes |
| Hold `Shift` + move mouse | Gold constellation cursor trail (desktop) |

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
git add .
git commit -m "update"
git push
```

Live at: **https://rushilswork.github.io**

---

## License

MIT — feel free to use as inspiration. Please don't copy directly.

---

*Built with care. Designed to be fast, accessible, and memorable.*