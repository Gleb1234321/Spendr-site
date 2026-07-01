# Spendr — landing page

Marketing site for **Spendr**, a fast, private, local-first expense tracker
(keypad → tap a category). Static site, served via **GitHub Pages**.

## Pages
- `index.html` — landing page (hero, how-it-works, features, screenshots, pricing).
- `privacy.html` — Privacy Policy (GDPR / UK GDPR / CCPA-CPRA, worldwide).
- `terms.html` — Terms of Use (worldwide, incl. Apple/Google app-store clauses).

## Design
Mirrors the app's design tokens (`lib/design.dart` in the app repo):
Bodoni Moda (serif, for numbers/headings) + Inter (UI); pure black-and-white
light theme, graphite + blue dark theme; coral-red brand accent. Includes a
persisted light/dark theme toggle.

## Assets
- `assets/logo-disc.png`, `assets/favicon.png` — logo mark (transparent).
- `assets/screens/*.jpg` — optimised app screenshots.

## Local preview
```bash
python -m http.server 8000   # then open http://localhost:8000
```

## Deploy
Pushing to `main` publishes automatically once GitHub Pages is enabled
(Settings → Pages → Branch: `main` / root). `.nojekyll` disables Jekyll
processing so all files are served as-is.
