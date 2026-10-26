# Circle — BGA Parent Community (Georgian)

One-page website of Circle, the parent loyalty programme of the
British-Georgian Academy (BGA): exclusive offers from partner businesses
across Georgia for BGA families. The whole site is in Georgian; it mirrors
circle.bist.ge (the BIST edition) and shares the same partner network.

## Structure

- `index.html` — the site (a single self-contained page; offers live in the
  `OFFERS` array near the bottom, UI strings follow the Circle Georgian
  localisation sheet)
- `support.js` — page runtime (renders the page content and interactions)
- `image-slot.js` — image slot component used by the page
- `logos/` — partner logos (each offer card shows its logo in a fixed-size
  container, so any logo size fits automatically)
- `photos/` — hero photographs
- `brand/` — Circle logo files and favicon

## Deployment

The site is served by GitHub Pages directly from this branch (Settings →
Pages → Deploy from a branch) at <https://circle.bga.ge>. Every push
redeploys it automatically; the `.nojekyll` file makes Pages publish the
files as-is without a Jekyll build.

To view locally, serve the folder with any static file server, e.g.:

```sh
python3 -m http.server
```

then open <http://localhost:8000>.
