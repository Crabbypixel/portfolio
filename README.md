
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
## Notes

- Light and dark themes are driven by `prefers-color-scheme`, with a toggle in the
  header that stores the choice in `localStorage`.
- Type is Archivo, IBM Plex Sans and IBM Plex Mono, loaded from Google Fonts with
  system fallbacks.
