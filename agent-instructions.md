# Agent Instructions

This repository is the public website of the Open Health Technology Foundation (OHTF), built with Zensical and deployed to GitHub Pages at openhealthtechnology.org. It is not OHTF's planning repository and holds no project code.

This file is the entry point for AI coding agents. Read it before changing anything.

## Read First

- [README.md](README.md) - layout, setup and checks.
- [CONTRIBUTING.md](CONTRIBUTING.md) - writing style.
- [pacharanero/house-style](https://github.com/pacharanero/house-style) - cross-repo standards, especially `docs.md` (Zensical, Pages deploy), `ui.md` (interface design) and `ci.md` (action pinning, Dependabot).
- OHTF planning material (governance, legal, roadmap) is the upstream source of truth for what this site says. It lives outside this repository; ask the maintainer where if you need it.

## Core Invariants

- The registered company is **Open Health Technology CIC**, company number 17544421, incorporated 27 October 2026. "Open Health Technology Foundation CIC" is the intended later name, pending sensitive-word approval; never present it as the registered name until the rename is filed. Keep the footer's legal disclosures (registered name, number, place of registration) accurate. The registered office address (the accountant's office) is deliberately omitted from the footer until an AD01 corrects its postcode on the register (M33 5SD was entered in error; the correct postcode is M33 3SD); add it back to the footer, and correct the Governance page, once that change is registered.
- Published legal documents under `docs/transparency/` are reproduced verbatim from what was filed. Never edit their wording; redact personal data only, and say so.
- Write about OHTF as a business-as-usual operation. Do not track the organisation's own progress on the site: no "intend to", "will be confirmed", "draft", "in preparation", "being set up", "so far" or founding-timeline status updates. State what OHTF is and does in the present tense. The only permitted in-progress statement is the one-line note that a change of name to Open Health Technology Foundation CIC is in progress.
- Foundation Projects are those whose repositories live under github.com/ohtf; `oct` (Open Clinical Terminology) was the first and the `nhs-number` Python package (`ohtf/nhs-number-py`) the second. Never present a candidate project as owned or maintained by OHTF; label candidates as candidates.
- Do not publish confidential planning material: partner negotiations, named director or non-executive candidates, customer information, procurement documents.
- Every page under `docs/` appears in `nav:` in `mkdocs.yml`.
- Advisers are listed only with their agreement to be named and pictured, and the Advisers page is never published with an empty list. Follow [Adding an adviser](#adding-an-adviser) for every one.
- Brand colours are defined once, as tokens at the top of `docs/stylesheets/extra.css`: Surgical Green (`#0D4A3B`) and its white-mixed tint scale (80, 60, 40, 20, 10), from OHTF's branding reference in the planning material. No accent or complementary colours have been chosen; do not introduce any, or any other near-matching greens. For depth, use black or white at low opacity over a brand colour. Keep text and interactive states at WCAG AA contrast or better.
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
- `s/headshot <photo> <slug> [gravity]` - turn a supplied photo into an adviser headshot in `docs/assets/advisers/`.
- `s/check-docs-nav` - fail on orphaned or missing nav pages.

## Adding an adviser

Use this procedure for every adviser, in this order.

1. **Record them in the planning material.** In `team/advisors.md` in the OHTF planning folder (ask the maintainer where it is), add them under `## Confirmed`, as a `### <display name>` heading with their details below: display name (including any title), role, photo source, and the date added. Check they are already in that file's "Listed Advisers" consent list; if not, stop and ask. Never record private contact details there.
2. **Make the headshot.** Download the supplied photo into its own new, empty temporary directory, then run `s/headshot <photo> <slug>` (slug is their name in lowercase hyphen-case, for example `michael-barton`). Every photo goes through `s/headshot`, never by hand, so all headshots share the same monochrome treatment, evened-out tonality, square crop and stripped metadata. Open the result and check the face is not cut off; if it is, rerun with `north` or another gravity.
3. **Add them to the site.** Append an entry to the `advisers:` front matter of `docs/about/advisers.md`, with `name`, `role` and `photo: assets/advisers/<slug>.jpg`. Use the name and role exactly as recorded in step 1.
4. **Check and commit.** Run the checks below, inspect the Advisers page at phone, tablet and desktop widths in light and dark schemes, and commit with a message like `feat(about): add <name> as an adviser`.

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
