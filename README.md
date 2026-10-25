# Drenched — site files

## Adding the fonts
Neither Sunbird nor Bakso Sapi is on Google Fonts, so the page can't pull them
automatically — you need to add the actual font files yourself:

1. Get licensed copies of both fonts (remember: Sunbird's free version is
   personal-use-only and explicitly bans use in games — you'll need the paid
   license from hanodedfonts.com for commercial use; Bakso Sapi's free
   license does appear to allow commercial use, but double-check current terms).
2. Convert/export them to `.woff2` (best web performance) and drop the files
   into `assets/fonts/`, named:
   - `assets/fonts/Sunbird-Regular.woff2`
   - `assets/fonts/BaksoSapi-Regular.woff2`
3. Refresh the page — the real fonts will load automatically. Until then, the
   site uses close fallback fonts so it still looks reasonable.

## Adding images
Every image on the site is currently a dashed placeholder box labeled
"+ Add image" with a suggested size. To replace one:
- Open `index.html` (or `meet-the-team.html`) in any text editor
- Find the `<div class="img-placeholder">...</div>` block you want to replace
- Swap it for a normal `<img src="assets/images/your-file.jpg" alt="...">`
- Drop your image file into `assets/images/`

## What's next
This is the static front-end only. The natural next step is wiring up a free
CMS (Decap or Tina) so the director can edit text, screenshots, and add new
DLC/update entries from a simple dashboard instead of editing HTML directly —
happy to set that up whenever you're ready.
