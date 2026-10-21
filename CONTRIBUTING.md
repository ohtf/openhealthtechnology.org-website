# Contributing

Thanks for helping improve the OHTF website.

- Small fixes: use the edit link on the page, or open a pull request.
- Larger changes, or anything that changes what OHTF says about its governance, legal status or projects: open an issue first so it can be discussed.
- Sign off every commit under the [Developer Certificate of Origin](https://openhealthtechnology.org/community/dco/): `git commit -s`.
- Follow the [code of conduct](https://openhealthtechnology.org/community/code-of-conduct/).

## Writing style

- British English.
- Direct and concrete. Name the thing and the action; avoid marketing filler.
- Use hyphens, not em dashes.
- Do not hard-wrap Markdown paragraphs.
- Never describe OHTF as incorporated, or a project as an OHTF project, until that is true.

## Before opening a pull request

```sh
s/check-docs-nav
s/build --strict
```

Add every new page to `nav:` in `mkdocs.yml`, or the nav check fails.
