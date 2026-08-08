# s-sayan.github.io

Personal academic website of Sayan Saha, Postdoctoral Research Associate at Northeastern University.

Live at [s-sayan.github.io](https://s-sayan.github.io).

## Built with al-folio

This site is built on [**al-folio**](https://github.com/alshedivat/al-folio), a Jekyll theme for academic websites, released under the MIT License. The starter's `v1.x` "thin starter" architecture keeps layouts, includes, Sass, and feature runtime (search, math, CV rendering, citations, icons, etc.) in versioned gems (`al_folio_core` and friends); this repository holds only the site's own configuration, content, and data:

- `_config.yml` — site settings and plugin/theme wiring
- `_pages/` — About, CV, Publications, Outreach
- `_data/` — CV data, social links, plugin catalog metadata
- `_bibliography/` — publication list (BibTeX)
- `assets/` — profile photo, outreach photos, CV PDF

## Structure notes

- `/blog/` and `/misc/` are self-contained static sub-sites, served as-is by Jekyll (not built from al-folio's own blog/post system).
- `docs/` holds the LaTeX source and PDF for the CV.
- The site deploys via GitHub Actions (`.github/workflows/deploy.yml`) to GitHub Pages.

## Local development

This repo requires Ruby (Bundler) and Node to build:

```bash
bundle install
npm ci
bundle exec jekyll serve
```
