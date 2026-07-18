# abehrouz.github.io

Personal academic website of **Ali Behrouz** — a modern, minimal, dependency-free static site.
No Jekyll, no build step: what you see in this repo is exactly what GitHub Pages serves.

## Structure

```
├── index.html              # Home: bio, selected publications, podcasts, service
├── publications/           # Full publication list, grouped by year
├── awards/                 # Selected awards
├── talks/                  # Invited talks
├── datasets/               # Released datasets + BibTeX
├── OpenAtlas/              # OpenAtlas project page (standalone, self-contained)
├── assets/style.css        # All styling (colors, spacing, typography)
├── images/                 # Profile photo, favicon
├── files/                  # PDFs (e.g., NL.pdf)
└── .nojekyll               # Tells GitHub Pages to skip Jekyll processing
```

## Editing

- **Colors / fonts / spacing** — everything is controlled by the CSS variables at the top of
  `assets/style.css` (`--accent`, `--ink`, `--maxw`, ...). Change `--accent` to re-theme the
  whole site in one line.
- **Add a publication** — copy an existing `<li class="pub">...</li>` block in
  `publications/index.html` (and `index.html` if it should appear under Selected Publications)
  and edit the title, authors, venue chip, and links. Chip styles: `chip` (blue, venues),
  `chip preprint` (gray, arXiv), `chip award` (amber), `chip media` (violet, press).
- **Add a podcast** — copy a `<div class="podcard">` block in `index.html`.
- **CV** — the nav "CV" button points to a Google Drive link; update the URL in the header of
  each page (or point it to a PDF in `files/`).

## Deploying

Push to the `master`/`main` branch of `ABehrouz/ABehrouz.github.io` — GitHub Pages publishes
it automatically at https://abehrouz.github.io/.
