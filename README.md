# acadiaridgelp.com

Static website for Acadia Ridge LP, hosted on GitHub Pages. No build step.

## Publish
1. Put these files at the root of the repository (keep `CNAME` and `.nojekyll`).
2. Settings → Pages → Build and deployment → "Deploy from a branch" → `main` / `(root)`.
3. Custom domain: `acadiaridgelp.com` (read from `CNAME`). Tick "Enforce HTTPS" once the certificate is issued.

## DNS (at the domain registrar)
- `A` records for `@`: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
- `CNAME` for `www`: `<your-github-username>.github.io`
- Remove any old A/CNAME records pointing to the previous host.

## Editing
- Copy lives in `index.html`; styles in `styles.css`.
- If the description changes, update the `<meta name="description">`, `og:description`, `twitter:description` and JSON-LD `description` together.
- Update `<lastmod>` in `sitemap.xml` when content changes.
- Investor Login links go directly to the NAV Fund Services portal.
- Photos rotate on each visit (night sky, winter summit, Bass Harbor). The list lives in the small script at the top of `index.html`; to add one, add WebP/JPG files to `assets/` and a line to that list.
- `site.js` handles the sticky header border, the mobile menu and the back-to-top button. The site still works if JavaScript is off.
