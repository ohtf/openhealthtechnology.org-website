# openhealthtechnology.org

The website of the Open Health Technology Foundation (OHTF): a neutral home for small, reusable, open-source health technology components.

[![CI](https://github.com/ohtf/openhealthtechnology.org-website/actions/workflows/ci.yml/badge.svg)](https://github.com/ohtf/openhealthtechnology.org-website/actions/workflows/ci.yml)
[![Licence: CC BY-SA 4.0](https://img.shields.io/badge/Licence-CC%20BY--SA%204.0-blue.svg)](LICENSE)

Live site: <https://openhealthtechnology.org>

## Quick start

Prerequisites: Python 3.10 or newer.

```sh
python3 -m venv .venv
./.venv/bin/pip install -r requirements.txt
s/docs
```

`s/docs` serves the site with live reload on the first free port between 8000 and 8030 and opens your browser.

## What it is

A static site built with [Zensical](https://zensical.org/) and deployed to GitHub Pages. It has a custom landing page (after the Material for MkDocs `home.html` pattern), and everything else is ordinary Markdown documentation: about, projects, services, governance, community policies and contact.

It is not the planning or governance working repository for OHTF, and it holds no project code. Foundation Projects live in their own repositories under [github.com/ohtf](https://github.com/ohtf).

## Layout

| Path | Purpose |
| --- | --- |
| `mkdocs.yml` | Site configuration and navigation. Every page must be in `nav:`. |
| `docs/` | Page content in Markdown. |
| `docs/index.md` | Landing page. Hero copy lives in its `hero:` front matter. |
| `docs/stylesheets/extra.css` | Brand colour tokens and landing-page styles. |
| `docs/assets/ohtf-mark.svg` | Placeholder mark until OHTF has a designed logo. |
| `docs/CNAME` | Custom domain for GitHub Pages. |
| `overrides/home.html` | Landing-page template. |
| `s/` | Repeated tasks: `s/docs` (serve), `s/build` (build), `s/check-docs-nav` (nav orphan check). |

## Checks

```sh
s/check-docs-nav
s/build --strict
```

CI runs both on every pull request. Pushes to `main` that touch the site deploy automatically via `.github/workflows/docs.yml`.

## Contributing

Corrections and improvements are welcome: use the edit link on any page, or open a pull request. Sign off your commits (`git commit -s`) under the [Developer Certificate of Origin](https://openhealthtechnology.org/community/dco/). See [CONTRIBUTING.md](CONTRIBUTING.md).

## Licence

All content and code in this repository is licensed under [CC BY-SA 4.0](LICENSE), copyright Open Health Technology Foundation contributors. Third-party marks and project names belong to their respective owners.
