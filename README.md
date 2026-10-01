# Taxkeeping LLC website

One-page static site for Taxkeeping LLC. No build step. Plain HTML, CSS, and JavaScript.

## Files
- `index.html`: the website
- `favicon.svg`: browser tab icon
- `assets/taxkeeping-logo.svg`: full logo (mark and wordmark)
- `404.html`: shown for missing pages
- `_headers`: security and caching headers for Cloudflare
- `robots.txt`: allows search engines to index the site

## Deploy on Cloudflare
1. Push these files to the root of a GitHub repository.
2. In the Cloudflare dashboard, go to **Workers & Pages**, then **Create**, then **Pages**, then **Connect to Git**, and pick the repository.
3. Use these build settings:
   - Framework preset: **None**
   - Build command: *(leave empty)*
   - Build output directory: `/`
4. Click **Save and Deploy**.
5. Under **Custom domains**, add `taxkeepingllc.com` (and `www.taxkeepingllc.com`).

Every push to the main branch redeploys the site automatically.

## Contact form
The form sends submissions to candy@taxkeepingllc.com through [FormSubmit](https://formsubmit.co).

The first submission from the live site triggers an activation email to that address. Click the link in that email to start receiving messages.

To change the recipient, search `index.html` for `candy@taxkeepingllc.com` and update both places it appears.
