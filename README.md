# masato-ishii-mi141.github.io

Personal website of Masato Ishii, built with [al-folio](https://github.com/alshedivat/al-folio) (Jekyll) and published on GitHub Pages.

- English (main): `/` — `_pages/about.md`
- Japanese: `/ja/` — `_pages/ja.md`

## How to update

| What | Where |
| --- | --- |
| Papers (shared by both languages) | `_bibliography/papers.bib` — entries with `selected = {true}` are shown, in file order |
| Paper thumbnails | `assets/img/publication_preview/` — referenced by the `preview` field |
| Venue badge colors | `_data/venues.yml` — keyed by the `abbr` field |
| Career, talks, awards, service | `_pages/about.md` (English) and `_pages/ja.md` (Japanese) |
| Profile photo | `assets/img/prof_pic.jpg` |
| Social icons (Scholar, X, LinkedIn) | `_data/socials.yml` |
| Site-wide settings | `_config.yml` |

## Deployment

Pushing to `main` runs `.github/workflows/deploy.yml`, which builds the site and pushes the output to the `gh-pages` branch.
In the repository settings, set **Pages → Build and deployment → Source** to **Deploy from a branch**, branch `gh-pages`, folder `/ (root)`.

## Local preview

```bash
bundle install
bundle exec jekyll serve   # http://localhost:4000/
```

The build needs a UTF-8 locale (e.g. `export LANG=C.UTF-8`) and ImageMagick for responsive images.

## License

The site template is al-folio, released under the MIT License (see `LICENSE`).
