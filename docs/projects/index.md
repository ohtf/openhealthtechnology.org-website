---
description: Foundation Projects, candidate projects and experimental projects at the Open Health Technology Foundation.
---

# Projects

**Foundation Projects** live at [github.com/ohtf](https://github.com/ohtf), with named maintainers and OHTF's [governance](../governance/index.md). **[Candidate projects](candidates.md)** are public, open-source projects going through [onboarding](bring-a-project.md); until they join, each is governed by its original home. When a project joins, its repository transfers to github.com/ohtf and the old address redirects. **Experimental projects** are early work started within OHTF that is not yet ready for use.

Each project's stage is defined in the [project lifecycle](../governance/project-lifecycle.md). Each Foundation Project has its own page with key facts, including its clinical safety and medical device position; see [why we publish so much](../transparency/why-we-publish.md).

## Foundation Projects

### `oct` - Open Clinical Terminology

An open, community-owned clinical terminology, developed clean-room from contributions by clinicians, developers and others. `oct` defines concept identifiers and internationalised descriptions; hierarchies are left to separate ontologies that reference `oct` identifiers.

**Status:** Incubating.

[Project page and key facts](oct.md) · [Website](https://openterminology.org/) · [Source](https://github.com/ohtf/oct)

### NHS Number (Python)

The `nhs-number` Python package validates, normalises, formats and generates NHS Numbers (including the Scottish CHI and Northern Irish H&C ranges), with region checks. A shared, language-agnostic set of test vectors lets any port to another language prove it gives the same answers.

**Status:** Incubating.

[Project page and key facts](nhs-number.md) · [Documentation](https://ohtf.github.io/nhs-number-py/) · [Source](https://github.com/ohtf/nhs-number-py) · [PyPI](https://pypi.org/project/nhs-number/)

### clincalc

Open, community-auditable clinical calculators. A single Rust engine computes every score, and every surface (command line, Python package, MCP tool, REST API, desktop and web interfaces) is driven from it, so a result is identical wherever it appears. Each calculator cites primary literature, is tested against published vectors and records its licence. It is published for software development, research, education and evaluation, not for making decisions about an individual patient's care on its own.

**Status:** Incubating.

[Project page and key facts](clincalc.md) · [Documentation](https://ohtf.github.io/clincalc/) · [Source](https://github.com/ohtf/clincalc)

### Digital PEWS

A charting and scoring component for the NHS National Paediatric Early Warning System (NPEWS) observation chart, built in plain HTML, CSS and JavaScript with no framework or build step, and integrating with electronic patient records through SMART on FHIR. It is a bounded component for a wider clinical system, not a complete EPR workflow. OHTF continues the project independently following the Royal College of Paediatrics and Child Health's indefinite pause of its PEWS work; existing attribution is retained. No clinically approved release has been designated; its clinical safety status is set out in the project's [`SAFETY.md`](https://github.com/ohtf/digital-pews/blob/main/SAFETY.md).

**Status:** Incubating.

[Project page and key facts](digital-pews.md) · [Demo](https://ohtf.github.io/digital-pews/demo) · [Source](https://github.com/ohtf/digital-pews)

## Candidate projects

Public, open-source projects proposed or invited to join OHTF and going through onboarding: NHS Number for Rust, sct, GitEHR, anarchie, Green Book, Medical Markdown, SAFETY.md and Clinicians Who Code: The Opinionated Handbook.

[See the candidate projects](candidates.md)

## Experimental projects

Early work started within OHTF and not yet proposed as a Foundation Project. Experimental projects are not ready for use and may change completely or stop.

### Panic Button

An open-source, LAN-first staff panic alarm for GP practices and other small workplaces.

[Project page and key facts](panic-button.md) · [Source](https://github.com/ohtf/panic-button)

## Not listed here?

If you maintain open-source health software that needs a neutral, long-term home, see [bring a project](bring-a-project.md).

Looking for something worth building? [Awesome Missing NHS Things](../about/awesome-missing-nhs-things.md) lists the software, data and infrastructure that NHS and UK health and care work needs but doesn't have.
