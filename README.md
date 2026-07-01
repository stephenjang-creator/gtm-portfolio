# Portfolio site

A single-page operator portfolio, deployed as a static site on GitHub Pages.

## Files
- `index.html` — the page (self-contained; fonts load from Google Fonts, with system fallbacks)
- `Stephen_Jang_Portfolio.png` — link-preview image (Open Graph / Twitter card)
- `.nojekyll` — tells GitHub Pages to serve files as-is (no Jekyll build)

Note: nothing here is downloadable by design. The one-pager is the web page itself,
and the full 90-day implementation plan is NOT published — the "Request the full
90-day implementation plan" button opens a pre-filled email (native mail client,
with a Gmail-compose fallback) so interested people reach out directly. Send the
plan manually in reply.

## Deploy in ~5 minutes

1. Create a new **public** repo on GitHub. For a personal site at
   `https://stephenjang.github.io`, name the repo exactly `stephenjang.github.io`.
   Any other name gives you `https://<user>.github.io/<repo>/` instead.
2. Upload all files in this folder to the repo root (drag-and-drop in the GitHub
   web UI works, or `git add . && git commit -m "portfolio" && git push`).
3. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a
   branch**, branch `main`, folder `/ (root)`. Save.
4. Wait ~1 minute. Your site is live at the URL shown on that Pages settings page.

## Custom domain (optional, ~$12/yr)
Buy a domain, then in **Settings → Pages → Custom domain** enter it and follow the
DNS instructions GitHub shows. Add a `CNAME` file (GitHub creates it for you) and
enable "Enforce HTTPS".

## Updating content
Edit `index.html` and re-commit. To refresh the PDFs, replace the files with the
same names. Keep the filenames identical so the links in `index.html` keep working.
