---
template: home.html
title: Open Health Technology Foundation
description: A neutral, long-term home for open-source health technology.
hide:
  - navigation
  - toc
hero:
  eyebrow: Open Health Technology Foundation
  title: A neutral, long-term home for open-source health software
  lead: >-
    OHTF stewards the open-source software that health care runs on, from
    NHS Number and SNOMED CT tooling and clinical calculators to Git-based
    health records. Open code, named maintainers, and an organisation that
    outlasts any one employer.
  actions:
    - label: See the projects
      link: projects/
    - label: Why OHTF exists
      link: about/why-ohtf/
  code:
    alt: "A terminal session installing the nhs-number Python library and validating an NHS Number, which returns True."
    caption: "nhs-number, one of OHTF's candidate projects. Talk is cheap; show me the code."
    lines:
      - prompt: "$"
        input: "pip install nhs-number"
      - prompt: "$"
        input: "python"
      - prompt: ">>>"
        input: "import nhs_number"
      - prompt: ">>>"
        input: "nhs_number.is_valid(\"943 476 5919\")"
      - output: "True"
      - prompt: ">>>"
        input: "nhs_number.is_valid(\"1234567890\")"
      - output: "False"
---

# Open Health Technology Foundation

<div class="ohtf-status" markdown>

**Status:** OHTF is preparing to incorporate as Open Health Technology Foundation CIC, a UK community interest company. Until then it operates as an open working group around [github.com/ohtf](https://github.com/ohtf). [Read the governance position](governance/index.md).

</div>

## The gap OHTF fills

Health technology has standards bodies, professional bodies, policy organisations and large general-purpose software foundations. None of them is a practical, health-specific home for the open-source software that working developers and clinicians actually depend on: libraries, terminology tools, clinical calculators and record systems. That software is too important to leave in someone's personal GitHub account, or in an employer's organisation that might disappear. [More on why OHTF exists](about/why-ohtf.md).

## What OHTF looks after

OHTF accepts open-source projects that meet four tests:

<div class="ohtf-criteria" markdown>

<dl markdown>
<dt>Vendor-neutral</dt>
<dd>Useful across products, organisations and countries, not tied to one vendor or one national architecture.</dd>
</dl>

<dl markdown>
<dt>Built for implementers</dt>
<dd>Working code for developers and clinicians, rather than policy papers or standards artefacts.</dd>
</dl>

<dl markdown>
<dt>Open and maintained</dt>
<dd>Published under an open licence with named maintainers, a security contact and a clear lifecycle status.</dd>
</dl>

<dl markdown>
<dt>Worth keeping</dt>
<dd>Software the health system would find costly and risky to lose, or to keep reinventing.</dd>
</dl>

</div>

## The first projects

These projects are expected to be among the first to join. They are already public and in active development, and each one moves into OHTF once it has named maintainers and has been through [project onboarding](projects/bring-a-project.md).

| Project | What it does |
| --- | --- |
| [NHS Number](projects/index.md#nhs-number) | Validate, normalise and generate NHS Numbers, in Python and Rust. |
| [sct](projects/index.md#sct) | A local-first SNOMED CT toolchain: from RF2 release to SQL, Parquet, Markdown and fast local queries. |
| [clincalc](projects/index.md#clincalc) | Open, auditable clinical calculators, each citing primary literature and tested against published vectors. |
| [GitEHR](projects/index.md#gitehr) | A decentralised, multi-contributor electronic health record that uses Git as its storage layer. |
| [anarchie](projects/index.md#anarchie) | A complete openEHR clinical data repository with Git-tracked, file-based persistence. |

[See all projects](projects/index.md){ .md-button }

## How a project joins

<ol class="ohtf-steps" markdown>
<li markdown>**Propose it.** Open a discussion on GitHub describing the project, its users and who maintains it. [How to propose a project](projects/bring-a-project.md).</li>
<li markdown>**Name the maintainers.** Every Foundation Project needs at least one named maintainer, a contribution path and a security contact.</li>
<li markdown>**Adopt the basics.** An open licence, the [code of conduct](community/code-of-conduct.md), [DCO sign-off](community/dco.md) on contributions and a [security policy](community/security.md).</li>
<li markdown>**Move it under OHTF.** The repository transfers to [github.com/ohtf](https://github.com/ohtf), with OHTF holding domains and trademarks where that protects the project's neutrality.</li>
</ol>

## Hosting, support and training

Some health organisations need more than code: a hosted API, an assured deployment, support with a named contact, or training for their team. OHTF can provide these as paid services. The income pays for maintenance, and the underlying code stays open. [About OHTF services](services.md).

## Get involved

- **Use the projects** and report what breaks. Issues on GitHub are the fastest route.
- **Contribute code or documentation.** Start with [contributing to OHTF projects](community/index.md).
- **Bring a project** that needs a neutral, long-term home: [propose a project](projects/bring-a-project.md).
- **Talk to us** about partnership, hosting or support: [contact OHTF](contact.md).
