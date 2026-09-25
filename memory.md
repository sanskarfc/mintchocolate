# memory.md

## Project
- Repo: sanskarfc/mintchocolate (private)
- Static Vercel site, `outputDirectory: public`
- Homepage: `public/index.html` — full-screen layered scene, no visible text

## Scene layers (all same canvas/size, cover + centered)
- Background: `public/Bgmintchoc.png` via CSS on `html`
  (`background: #ff8c00 url("Bgmintchoc.png") no-repeat center center fixed; background-size: cover`)
- Mid: `public/catmint.gif` (transparent) — `.center-gif`, fixed inset 0, 100vw x 100svh, object-fit cover
- Top: `public/sparksmint.gif` (transparent) — `.full-gif`, same full-screen cover
- Roaming SVG cats + `<h1>hi medha</h1>` removed; `<title>` kept for CI

## Notes
- CI: `.github/workflows/ci.yml` validates vercel.json + inline JS (no inline script left)
- Custom ice-cream SVG cursor kept on `html`
