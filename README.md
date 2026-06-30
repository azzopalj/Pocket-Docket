# Pocket Docket — Website

Static marketing landing page (`index.html`) and privacy policy (`privacy.html`) for Pocket Docket.
No build step — just plain HTML/CSS. Host anywhere; instructions below are for free GitHub Pages.

## Option A — User site (cleanest URLs)

Serves at `https://azzopalj.github.io/`.

1. Create a new GitHub repo named exactly **`azzopalj.github.io`** (public).
2. Put `index.html` and `privacy.html` in the repo root and push:
   ```bash
   cd website
   git init
   git add index.html privacy.html
   git commit -m "Add Pocket Docket site"
   git branch -M main
   git remote add origin https://github.com/azzopalj/azzopalj.github.io.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, Branch: **main / (root)**, Save.
4. Wait ~1 minute. Your URLs:
   - **Marketing URL:** `https://azzopalj.github.io`
   - **Privacy Policy URL:** `https://azzopalj.github.io/privacy.html`

## Option B — Project site

If you'd rather keep it in a named repo (e.g. `pocket-docket`):

1. Create a public repo, e.g. **`pocket-docket`**, push the two files.
2. **Settings → Pages → Source: Deploy from a branch → main / (root)**.
3. URLs:
   - **Marketing URL:** `https://azzopalj.github.io/pocket-docket/`
   - **Privacy Policy URL:** `https://azzopalj.github.io/pocket-docket/privacy.html`

## Put the URLs in App Store Connect

- **Marketing URL** → the home page URL above.
- **Privacy Policy URL** → the `privacy.html` URL above. (Required for submission.)

## Notes

- The logo is an inline SVG that recreates the app icon — no image files needed.
- Update the "Last updated" date in `privacy.html` whenever you change the policy
  (e.g. if you add analytics later — currently the app uses none).
- The App Store links point to app id `6785915346`; they work once the app is live.
