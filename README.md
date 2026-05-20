# Varun Nair — Personal Site

A single-file static site. No build step, no dependencies.

## Deploy to Render (free, ~2 minutes)

1. Push these files to a GitHub repo (e.g. `varun-site`).
2. Go to https://dashboard.render.com → **New +** → **Static Site**.
3. Connect your GitHub repo.
4. Fill in:
   - **Build Command:** *(leave blank)*
   - **Publish Directory:** `.`
5. Click **Create Static Site**.

Render will give you a `*.onrender.com` URL.

## Use your own `.dev` domain

1. Buy the domain on [Google Domains / Squarespace](https://domains.google) or [Porkbun](https://porkbun.com) (`.dev` requires HTTPS, which Render handles automatically).
2. In Render → your site → **Settings** → **Custom Domains** → add `yourname.dev`.
3. Render will show you a `CNAME` (or `A`) record. Add it in your domain registrar's DNS settings.
4. Wait 5–30 minutes for DNS to propagate. Render auto-issues a Let's Encrypt SSL cert.

## Editing

Everything lives in `index.html`. Colors, fonts, and spacing are CSS variables at the top:

```css
:root {
  --bg: #f4f1ea;      /* warm off-white */
  --ink: #1a1a1a;     /* near-black */
  --accent: #c8553d;  /* terracotta */
}
```
