# SprayLog — PWA Package

This folder contains everything you need to host SprayLog as an installable Progressive Web App (PWA).

## Files
- `index.html` — entry page. Paste your app markup/JS here (or replace with your full app file).
- `manifest.json` — PWA manifest (icons, theme color, start URL).
- `service-worker.js` — offline cache.
- `icons/` — required app icons.

## Quick Deploy
### GitHub Pages
1. Create a new repo (e.g., `spraylog`).
2. Upload these files at the repo root.
3. Settings → Pages → Deploy from branch → `main` → `/root`.
4. Open the site on your phone and **Install/Add to Home Screen**.

### Netlify / Vercel
- Drag‑and‑drop this folder into Netlify, or run `vercel deploy` from this folder.

## Notes
- Make sure the site is served over **HTTPS**.
- After first load online, it will work **offline** thanks to caching.
- To push an update: change something in `service-worker.js` (e.g., bump `CACHE` version) and redeploy.
