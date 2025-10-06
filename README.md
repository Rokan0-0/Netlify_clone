# Netlify_clone

A small static clone / landing page inspired by Netlify. The project contains a single-page HTML + CSS site
with images and a hero SVG illustration. It is intended as a practice project for layout, SVG usage, and
CSS animations.

## What you'll find here
- `index.html` — the main page markup
- `style.css` — styles and animations
- `images/` — project images (logo and hero assets)

## Quick preview (locally)
You can preview this site by opening `index.html` directly in a browser. For a slightly better local server
experience (useful for testing paths and CORS with external assets), use a tiny static server. Example using
Python (if installed):

```powershell
cd 'C:\Users\USER\Desktop\netlify'
# Python 3
python -m http.server 8000
# then open http://localhost:8000 in your browser
```

## Suggestions & notes
- The hero SVG is currently inlined in `index.html` which makes the file very large — consider moving it to
	`images/hero.svg` and referencing it with an `<img>` for readability and caching.
- There were duplicate Google Fonts `preconnect` tags; keep only one pair and request all fonts in a single URL.
- `<marquee>` is deprecated — consider replacing it with a CSS or JS-based marquee/slider for accessibility.
- Add a `.gitignore` to avoid committing editor settings or build artifacts (e.g., `.vscode/`, `node_modules/`).

## Contribution
Small fixes (readability, accessibility, performance) are welcome. If you plan a larger change, open an issue
or a draft PR so we can discuss goals (e.g., responsive refactor, swapping the SVG for a lightweight PNG, or
adding a mobile-first breakpoint system).

---
Made with ❤️ — feel free to clone and experiment.
