# danielmccrummen.com

One-page portfolio site for Daniel McCrummen, built with Jekyll and hosted on GitHub Pages.

## Updating content

Almost everything you'd change lives in **`_data/site.yml`**:

- **Bio, title, studio** — `role`, `studio`, `bio`
- **Reels** — set `vimeo_id` and `vimeo_hash` (the `h=` value from Vimeo's embed link), then update the `breakdown` or `chapters` list
- **Resume** — replace `assets/Daniel_McCrummen_Resume.pdf` (same filename) or point `resume` at a new file
- **Links and email** — `links`, `email`

Push to `master` and GitHub Pages rebuilds the site in a minute or two.

## Files

- `index.html` — the page layout
- `_layouts/default.html` — header, footer and `<head>`
- `assets/css/site.css` — all styling (colors are variables at the top)
- `resume/` — keeps the old `/resume/` link working by redirecting to the PDF

## Preview locally (optional)

```
bundle install
bundle exec jekyll serve
```
