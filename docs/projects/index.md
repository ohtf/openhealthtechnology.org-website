---
description: Foundation Projects and candidate projects at the Open Health Technology Foundation.
---

# Projects

**Foundation Projects** live at [github.com/ohtf](https://github.com/ohtf), with named maintainers and OHTF's [governance](../governance/index.md). **Candidate projects** are public, open-source projects going through [onboarding](bring-a-project.md); until they join, each is governed by its original home, linked below. When a project joins, its repository transfers to github.com/ohtf and the old address redirects.

Each project's stage is defined in the [project lifecycle](../governance/project-lifecycle.md).

## Foundation Projects

### `oct` - Open Clinical Terminology

An open, community-owned clinical terminology, developed clean-room from contributions by clinicians, developers and others. `oct` defines concept identifiers and internationalised descriptions; hierarchies are left to separate ontologies that reference `oct` identifiers.

**Status:** Incubating.

[Website](https://openterminology.org/) · [Source](https://github.com/ohtf/oct)

### NHS Number (Python)

The `nhs-number` Python package validates, normalises, formats and generates NHS Numbers (including the Scottish CHI and Northern Irish H&C ranges), with region checks. A shared, language-agnostic set of test vectors lets any port to another language prove it gives the same answers.

**Status:** Incubating.

[Documentation](https://ohtf.github.io/nhs-number-py/) · [Source](https://github.com/ohtf/nhs-number-py) · [PyPI](https://pypi.org/project/nhs-number/)

### clincalc

Open, community-auditable clinical calculators. A single Rust engine computes every score, and every surface (command line, Python package, MCP tool, REST API, desktop and web interfaces) is driven from it, so a result is identical wherever it appears. Each calculator cites primary literature, is tested against published vectors and records its licence. It is published for software development, research, education and evaluation, not for making decisions about an individual patient's care on its own.

**Status:** Incubating.

[Documentation](https://ohtf.github.io/clincalc/) · [Source](https://github.com/ohtf/clincalc)

### Digital PEWS

A charting and scoring component for the NHS National Paediatric Early Warning System (NPEWS) observation chart, built in plain HTML, CSS and JavaScript with no framework or build step, and integrating with electronic patient records through SMART on FHIR. It is a bounded component for a wider clinical system, not a complete EPR workflow. OHTF continues the project independently following the Royal College of Paediatrics and Child Health's indefinite pause of its PEWS work; existing attribution is retained. No clinically approved release has been designated; its clinical safety status is set out in the project's [`SAFETY.md`](https://github.com/ohtf/digital-pews/blob/main/SAFETY.md).

**Status:** Incubating.

[Demo](https://ohtf.github.io/digital-pews/demo) · [Source](https://github.com/ohtf/digital-pews)

## Candidate projects

### NHS Number for Rust

The `nhs-number` Rust crate, by Joel Parker Henderson, implements the same NHS Number checks and is tested against the same shared vectors.

[Source](https://github.com/joelparkerhenderson/nhs-number-using-rust) · [crates.io](https://crates.io/crates/nhs-number)

### sct

A local-first SNOMED CT toolchain. One binary takes a raw RF2 release and turns it into NDJSON, SQLite, Parquet, Markdown, refsets and codelists, with fast local queries and tool use for LLMs, without depending on a terminology server.

[Documentation](https://pacharanero.github.io/sct/) · [Source](https://github.com/pacharanero/sct)

### GitEHR

A Git-based, decentralised, multi-contributor electronic health record. Clinical history is stored as files in a Git repository, inheriting Git's audit trail, integrity checks and offline working.

[Website](https://gitehr.org/) · [Source](https://github.com/gitehr/gitehr)

### anarchie

A complete openEHR clinical data repository, written in Rust, that uses Git-tracked flat files instead of a database server for persistence.

[Documentation](https://pacharanero.github.io/anarchie/) · [Source](https://github.com/pacharanero/anarchie)

### Green Book

The UK childhood immunisation schedule (Green Book chapter 11) is published as PDFs, and every system that needs it re-implements it by hand. This project provides a computable, versioned schedule and an engine that evaluates a patient's FHIR vaccination history against it, with a shared conformance suite across implementations.

[Documentation](https://pacharanero.github.io/greenbook/) · [Source](https://github.com/pacharanero/greenbook)

### Medical Markdown

An early-stage specification, with reference parsers, for writing free-text clinical notes in a lightweight Markdown-like syntax that can be parsed into structured, coded data using standard clinical headings.

[Documentation](https://pacharanero.github.io/medical-markdown/) · [Source](https://github.com/pacharanero/medical-markdown)

### SAFETY.md

A repository-native convention for clinical safety documentation. Like `README.md`, `LICENSE` and `SECURITY.md`, a root `SAFETY.md` puts the information reviewers, clinical safety officers and tools need where they will find it, next to the code, issues and releases that affect patient safety.

[Source](https://github.com/pacharanero/SAFETY.md)

### Clinicians Who Code: The Opinionated Handbook

A practical, opinionated guide for clinicians who want to build healthcare software safely, openly and quickly. Written by a clinician-developer, for clinician-developers.

[Read the handbook](https://pacharanero.github.io/clinicians-who-code-the-opinionated-handbook) · [Source](https://github.com/pacharanero/clinicians-who-code-the-opinionated-handbook)

## Not listed here?

If you maintain open-source health software that needs a neutral, long-term home, see [bring a project](bring-a-project.md).
