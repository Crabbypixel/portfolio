# Portfolio — Jaisurya Vetrivel

Personal portfolio site. One hand-written `index.html`: no framework, no build step,
no dependencies to install. Open the file and it runs.

**Live:** https://crabbypixel.github.io/portfolio/

## Structure

```
index.html                        the whole site (markup, styles, canvas script)
assets/Jaisurya_Vetrivel_Resume.pdf   résumé linked from the header and footer
.nojekyll                         tells GitHub Pages to serve the files as-is
```

## Running it locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

## Deploying

**GitHub Pages** — Settings → Pages → Source: *Deploy from a branch*, branch `main`,
folder `/ (root)`. The site is published at `https://<user>.github.io/portfolio/`.

**Vercel** — Import the repository at vercel.com/new and deploy with no settings
changed. It is a static site, so there is no framework preset, build command or
output directory to configure.

## Notes

- Light and dark themes are driven by `prefers-color-scheme`, with a toggle in the
  header that stores the choice in `localStorage`.
- The hero graphic is an isometric voxel field drawn on a `<canvas>`, a nod to
  [CrabbyGL](https://github.com/Crabbypixel/CrabbyGL). It holds still for anyone
  with `prefers-reduced-motion` set and pauses when the tab is hidden.
- Type is Archivo, IBM Plex Sans and IBM Plex Mono, loaded from Google Fonts with
  system fallbacks.
