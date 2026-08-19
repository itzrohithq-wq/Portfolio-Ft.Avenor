# Rohit — Avenor Studio portfolio

Static site. No build step: every file is served as-is.

## Files

| Path | What it is |
| --- | --- |
| `index.html` | Entry point — loading screen + CD player, imports the hero |
| `Hero.dc.html` | Hero, Hall of Mastery certificate grid, footer, certificate viewer |
| `Legal.dc.html` / `legal.html` | Privacy & Terms page (footer links point to `legal.html#privacy` / `#terms`) |
| `support.js` | Runtime that renders the pages — must stay next to the HTML files |
| `assets/` | Images, cursors, signature, artwork |
| `uploads/` | Audio tracks (mp3) and the 24 certificate PDFs |
| `.nojekyll` | Tells GitHub Pages to serve folders as-is |

## Deploy to GitHub Pages

1. Create a new repository on GitHub.
2. Upload the **contents** of this folder to the repository root (not the folder itself).
3. Settings → Pages → Source: `Deploy from a branch`, branch `main`, folder `/ (root)`.
4. Wait a minute, then open the URL Pages gives you.

## Notes

- Keep the folder structure. `assets/` and `uploads/` are referenced by relative paths.
- Certificate previews render through pdf.js loaded from a CDN, so the live site needs internet access.
- Audio starts on the first click (browsers block autoplay).
