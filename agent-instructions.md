# Agent Instructions

This repository is the public website of the Open Health Technology Foundation (OHTF), built with Zensical and deployed to GitHub Pages at openhealthtechnology.org. It is not OHTF's planning repository and holds no project code.

This file is the entry point for AI coding agents. Read it before changing anything.

## Read First

- [README.md](README.md) - layout, setup and checks.
- [CONTRIBUTING.md](CONTRIBUTING.md) - writing style.
- [pacharanero/house-style](https://github.com/pacharanero/house-style) - cross-repo standards, especially `docs.md` (Zensical, Pages deploy), `ui.md` (interface design) and `ci.md` (action pinning, Dependabot).
- OHTF planning material (governance, legal, roadmap) is the upstream source of truth for what this site says. It lives outside this repository; ask the maintainer where if you need it.

## Core Invariants

- Never state that OHTF is incorporated, a registered CIC, or able to contract until it is. Use "preparing to incorporate".
- Never present a candidate project as owned or maintained by OHTF.
- Do not publish confidential planning material: partner negotiations, named director or non-executive candidates, customer information, procurement documents.
- Every page under `docs/` appears in `nav:` in `mkdocs.yml`.
- Brand colours are defined once, as tokens at the top of `docs/stylesheets/extra.css`.
- Landing-page hero copy lives in `docs/index.md` front matter, not in `overrides/home.html`.
- British English, no em dashes, no hard-wrapped Markdown.

## Workflow

- `s/docs` - serve locally with live reload.
- `s/build` - build into `site/`.
- `s/check-docs-nav` - fail on orphaned or missing nav pages.

## Before Every Commit

```sh
s/check-docs-nav
s/build --strict
```

For visual changes, inspect the rendered site at phone (390x844), tablet (768x1024) and desktop (1440x900) widths, in light and dark schemes.

## Git Workflow

- Commit each validated, coherent change with a conventional commit message, signed off (`git commit -s`).
- Do not push unless the user asks.

## Approval Required

Ask before pushing, changing GitHub Pages or DNS settings, editing workflow permissions, or publishing anything that describes OHTF's legal status, governance or partners differently from the planning material.
