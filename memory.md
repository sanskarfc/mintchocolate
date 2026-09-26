# memory.md

## Project
- Repo: sanskarfc/mintchocolate (private)
- Static Vercel site, `outputDirectory: public`
- Homepage: `public/index.html` — scrollable two-screen scene, no visible text

## Scene (all same canvas/size, cover + centered)
- Page bg: `public/Bgmintchocver2.png` on `html` (fixed, cover)
- Hero (100svh spacer): pinned GIFs, `position: fixed; z-index: 0`
  - `public/catmint.gif` (transparent) — `.center-gif`
  - `public/sparksmint.gif` (transparent) — `.full-gif`
  - `public/choc1.png` — `.choc` (same full-viewport cover alignment)
- Scroll section (100svh, `z-index: 1`): `public/scrollbg.png` cover background,
  slides over the pinned layers while scrolling
  - `public/choc1.png`–`choc4.png` — `#choc.choc`, absolute cover in section, click-cycles 1→2→3→4→1
  - `public/allchoc.png` — `.allchoc`, absolute cover in section, pointer-events none
- Unused (untracked, not referenced): `public/choc2.png`–`choc5.png`, `public/Bgmintchoc.png`
- Roaming SVG cats + `<h1>hi medha</h1>` removed; `<title>` kept for CI

## Notes
- CI: `.github/workflows/ci.yml` validates vercel.json + inline JS (no inline script left)
- Custom ice-cream SVG cursor kept on `html`
