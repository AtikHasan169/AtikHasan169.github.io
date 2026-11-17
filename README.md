# Atik Hasan — Portfolio Website

Single-page portfolio personalised with Atik Hasan's GitHub photo and info.

## What's inside

- `index.html` — the whole site: hanging ID card, hero-reveal photo, GitHub stats, contact
- `venom.html` — the 3D "let's collab" goo button (WebGL, loaded in an iframe)
- `assets/avatar.jpg` — profile photo from https://github.com/AtikHasan169
- `assets/hero.jpg` — Spider-Man version of the same photo (same pose/background)
- `PROMPT.md` — professional prompt to rebuild this site in another builder (v0, Lovable, Bolt, Claude, ChatGPT)
- `LICENSE-portfolio-effects`, `LICENSE-venom-button` — keep these with the site

## Preview locally

```bash
python -m http.server 8000
```

Then open http://localhost:8000 — the 3D button needs a server; opening the file directly still shows the CSS pill version.

## Deploy to GitHub Pages (atikhasan169.github.io)

1. Open the `AtikHasan169.github.io` repo on GitHub.
2. Upload everything in this folder to the repo root (replace the old `index.html`).
3. Commit, wait a minute for Pages to publish, then open https://atikhasan169.github.io/

Vercel also works: import this folder as a static site, no build command needed.

## Changing things

- **Spider-Man reveal:** `assets/hero.jpg` is the Spider-Man edit. To change it, replace that file with another same-size, same-pose edit. The prompt used is in `PROMPT.md`, section 3.
- **ID card text:** edit `ID_CONFIG` at the top of the first `<script>` in `index.html`.
- **Collab button link:** edit `CONFIG.link` in the goo-button `<script>` in `index.html` (currently `#contact`).
