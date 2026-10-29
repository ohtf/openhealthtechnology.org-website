# Agent Instructions

This repository is the public website of the Open Health Technology Foundation (OHTF), built with Zensical and deployed to GitHub Pages at openhealthtechnology.org. It is not OHTF's planning repository and holds no project code.

This file is the entry point for AI coding agents. Read it before changing anything.

## Read First

- [README.md](README.md) - layout, setup and checks.
- [CONTRIBUTING.md](CONTRIBUTING.md) - writing style.
- [pacharanero/house-style](https://github.com/pacharanero/house-style) - cross-repo standards, especially `docs.md` (Zensical, Pages deploy), `ui.md` (interface design) and `ci.md` (action pinning, Dependabot).
- OHTF planning material (governance, legal, roadmap) is the upstream source of truth for what this site says. It lives outside this repository; ask the maintainer where if you need it.

## Core Invariants

- The registered company is **Open Health Technology CIC**, company number 17544421, incorporated 27 October 2026. "Open Health Technology Foundation CIC" is the intended later name, pending sensitive-word approval; never present it as the registered name until the rename is filed. Keep the footer's legal disclosures (registered name, number, place of registration, registered office) accurate.
- Published legal documents under `docs/transparency/` are reproduced verbatim from what was filed. Never edit their wording; redact personal data only, and say so.
- Never present a candidate project as owned or maintained by OHTF.
- Do not publish confidential planning material: partner negotiations, named director or non-executive candidates, customer information, procurement documents.
- Every page under `docs/` appears in `nav:` in `mkdocs.yml`.
- Brand colours are defined once, as tokens at the top of `docs/stylesheets/extra.css`.
- Landing-page hero copy lives in `docs/index.md` front matter, not in `overrides/home.html`.
- British English, no em dashes, no hard-wrapped Markdown.

## Voice

OHTF should read as principled and distinctive, not as a generic health tech consultancy. It also bids for work with conservative public-sector organisations such as NHS England, so the site must be safe for that audience.

- **Outspoken on principle.** State positions on ethics, governance and power plainly. Do not water them down into corporate neutrality.
- **Never punch down.** Criticise ideas, structures and the powerful, never individuals or the less powerful.
- **No reputational liabilities.** Nothing a cautious public-sector reader would see as a risk, such as references to hacktivist groups or illegal activity.
- **Respectful of peer organisations.** Comparisons with other bodies stay factual about what each is for, not dismissive.

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
