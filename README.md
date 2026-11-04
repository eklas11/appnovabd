# App Nova BD — SEO deployment pack

## Files
- `index.html` — updated original application file with metadata improvements. The existing app code is preserved.
- `robots.txt` — crawler access rules and sitemap location.
- `sitemap.xml` — currently lists the homepage only.
- `site.webmanifest` — basic installable web-app metadata.
- `browserconfig.xml` — legacy Windows tile configuration.
- `_redirects` — fallback rule for Netlify-compatible static hosting; not read by GitHub Pages or Render.
- `_headers` — security headers for Netlify-compatible static hosting; configure equivalent headers in other hosts.
- `404.html` — simple not-found page for static hosts.
- `humans.txt` — basic site information.
- `security.txt` — template; replace the placeholder contact with a monitored email before publishing.

## Deploy
1. Upload the contents of this folder to the repository's web root, not the containing folder itself.
2. Keep the main HTML named `index.html` for static hosting.
3. Ensure `favicon.png` exists at the site root. The existing HTML and manifest refer to it; this pack does not invent a logo file.
4. Confirm the public canonical domain. These files currently use `https://appnovabd.onrender.com/`.
5. Open `/robots.txt`, `/sitemap.xml`, `/site.webmanifest` and `/browserconfig.xml` after deployment to confirm they return successfully.
6. Add the site to Google Search Console, verify ownership, submit `https://appnovabd.onrender.com/sitemap.xml`, and inspect the homepage URL.

## Important SEO limitations
- Indexing is not guaranteed and SEO files alone cannot guarantee ranking.
- The app is client-rendered and product pages are opened through `?p=...`; the sitemap intentionally lists only the homepage rather than inventing product URLs.
- Dynamic metadata inserted after JavaScript runs may not be treated the same as server-rendered product pages. For reliable product-level SEO, create crawlable server-rendered/prerendered HTML pages with unique title, description, canonical URL, real product images, accurate Product structured data, and sitemap entries.
- Do not mark products as reviewed, in-stock, or highly rated unless the underlying data supports those claims.
- `robots.txt` is not an access-control mechanism. Protect admin/user data with Firebase Authentication and database security rules.
- `_redirects` and `_headers` are host-specific. GitHub Pages ignores them; Render behavior depends on the service type and configuration.
- Never put payment secrets, private API keys, passwords, or privileged credentials in client-side HTML.
