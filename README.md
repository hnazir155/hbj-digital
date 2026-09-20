# HBJ Digital — website files (Vercel ready)

Static site. No build step, no dependencies to install.

## Files
- `index.html` — the whole site (HTML, CSS and JavaScript in one file)
- `logo-light.png` — logo for the dark header
- `logo-dark.png` — logo for the yellow footer
- `favicon.png` — browser tab icon
- `og.png` — preview image shown when the link is shared

## Put it live (GitHub → Vercel)
1. Upload these 5 files to the root of your GitHub repo (not inside a folder).
2. In Vercel, open the **hbj-digital** project → **Settings → Git** → connect that repo.
3. Framework preset: **Other**. Build command: leave empty. Output directory: leave empty.
4. Deploy. Every future push to the main branch redeploys automatically.

## After the first deploy
- **Settings → Deployment Protection**: turn **Vercel Authentication** off, otherwise visitors are asked to log in.
- **Settings → Domains**: add `hbjdigital.com` when you're ready.
- If you change the domain, update the four `https://hbj-digital.vercel.app` links near the top of `index.html` (canonical, og:url, og:image, twitter:image) to the new domain.

## Editing later
- WhatsApp number and email: the `CONTACT` line near the bottom of `index.html`.
- The 3D engine (three.js) loads from a CDN, with a second CDN as backup. If both fail, the page falls back to a simple non-3D scene automatically.
