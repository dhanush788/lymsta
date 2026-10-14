# lymsta.com

Static site for **lymsta.com**, served by GitHub Pages. No build step, no
dependencies — each page is a single HTML file with its CSS inlined.

- `index.html` — the studio homepage
- `404.html` — the not-found page (its own page, no longer a copy of the homepage)
- `sitemap.xml` / `robots.txt`
- `CNAME` — binds the Pages site to `lymsta.com`. Do not edit or delete.
- `og.png` — social preview card (1200×630)
- `favicon.svg`

The only external request either page makes is to Google Fonts for Inter.

## Editing

Edit the HTML and push to `main`. Pages redeploys automatically.

### Adding a product

In `index.html`, find the block commented `PRODUCTS — PLACEHOLDER ENTRIES`.
There are three placeholder cards. For each one: replace the `<h3>` with the
product name, replace the `.card-desc` sentence, delete any platform badge
(`Web` / `Android` / `iOS`) that does not apply, and leave the status as
`In development` until it ships. Delete a whole `<article>` to remove a slot;
copy one to add another — the grid reflows on its own.

### Brand

Set in `:root` at the top of each file. The dot after the wordmark is the only
saturated colour on the page (`--accent: #8ab4ff`); keep it that way.

## Regenerating og.png

Rendered from an SVG with headless Chrome at 1200×630. Source lives in this
README's history only — recreate by screenshotting a page at that size if the
brand changes.
