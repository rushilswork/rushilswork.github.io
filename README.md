# rushilswork.github.io

> Personal portfolio — [rushilswork.github.io](https://rushilswork.github.io)

## About

Portfolio of **Rushil Pillamari**, Software Engineer based in Hyderabad, India. Single-file static site — no frameworks, no build tools, no dependencies. 94KB.

## Stack

- Vanilla HTML / CSS / JS — zero dependencies
- Playfair Display · Syne · JetBrains Mono (Google Fonts)
- CSS Scroll Timeline API (progress bar)
- CSS `clip-path` wipe (theme transition)
- CSS `perspective` + `transform-style: preserve-3d` (card flip)
- Canvas API (particle system + cursor trail)
- IntersectionObserver (scroll reveal)
- Device Motion API (shake detection)

---

## Features

### Design
- Preloader — animated R mark + progress bar
- Character-by-character hero name reveal
- Scroll-driven gold progress bar
- Film grain overlay
- Ghost section numbers 01–04
- Active nav highlight on scroll
- Back to top button
- Light / Dark mode — cinematic diagonal wipe transition
- Theme preference persisted via `localStorage`

### Animations
- Per-element scroll reveal — varied per section
- Skill tag stagger on reveal
- Stat counters animate on scroll
- Section label line draws in
- Hero orb parallax on mouse (desktop)
- Magnetic contact buttons (desktop)
- Gold glow sweep on project card hover
- 3D card flip on single click / tap

### Responsive
- 4 breakpoints: `480px` / `768px` / `1024px` / `1400px`
- Hamburger menu with fullscreen overlay on mobile
- Touch device optimisations throughout

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
| Shake device | Same dust dissolve effect |
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

```bash
# Open index.html directly, or serve locally
npx serve .
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
