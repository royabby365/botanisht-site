# Botanisht marketing site

The public website advertising **[Botanisht](https://github.com/royabby365/botanisht)** — the open-source, offline-first plant care companion.

This is a self-contained static site: plain HTML, CSS and vanilla JavaScript with **no build step and no external runtime dependencies** (Google Fonts is the only CDN link, with a system-font fallback).

## Local preview

```bash
# from this directory
python3 -m http.server 8000
# then open http://localhost:8000
```


Or just open `index.html` in a browser.

## Structure

```
index.html              # single-page site (hero, features, climate, hydroponics, platforms, open source, CTA)
assets/css/style.css    # theme + responsive styles (light/dark via [data-theme])
assets/js/main.js       # theme toggle, mobile nav, scroll reveal
assets/img/logo.svg     # favicon + brand mark
```

## Deploy (GitHub Pages)

The site is served from the repository root on the `main` branch. Enable Pages once:

1. Repo **Settings → Pages → Build and deployment → Source: Deploy from a branch**
2. Branch: `main`, folder: `/ (root)`
3. Save — the site publishes at `https://royabby365.github.io/botanisht-site/`

No GitHub Actions workflow is required.

## Editing

All copy lives in `index.html`. Feature content is grounded in the actual app source
(`lib/models/...`, `lib/widgets/hydroponic/...`, `lib/services/sensors/...`). Keep marketing
claims aligned with what the Flutter app actually implements.

## License

MIT — same as the Botanisht app.

[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/royabby)
