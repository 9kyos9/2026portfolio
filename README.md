# 2026portfolio

Personal portfolio built with [Jekyll](https://jekyllrb.com/) and hosted on GitHub Pages.

**Live site:** https://9kyos9.github.io/2026portfolio

## Structure

```
├── _config.yml         # Site config (title, nav, baseurl)
├── _layouts/
│   └── default.html    # Page shell (header, footer, nav)
├── _data/
│   └── projects.yml    # Project list — edit your projects here
├── assets/css/
│   └── style.css       # Styles (light + dark mode)
├── index.html          # Home page
├── projects.html       # Projects page
└── about.md            # About page
```

## Editing content

- **Projects:** edit `_data/projects.yml`
- **About:** edit `about.md`
- **Site title / nav / links:** edit `_config.yml`

## Run locally (optional)

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000/2026portfolio/

## Deploy

Push to the `main` branch. In the repo settings, enable **GitHub Pages**
(Settings → Pages → Source: *Deploy from a branch* → `main` / `root`).
