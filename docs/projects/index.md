---
description: Projects expected to join the Open Health Technology Foundation, and other candidates.
---

# Projects

These are real, public, open-source projects, mostly started by people involved in founding OHTF. Being listed here is not a claim that OHTF already owns or maintains a project. Each one becomes a Foundation Project when it has named maintainers and has completed [onboarding](bring-a-project.md).

Each entry links to where the code lives today. When a project moves under OHTF, its repository transfers to [github.com/ohtf](https://github.com/ohtf), and the old address redirects.

!!! info "Lifecycle status"

    All projects below are currently at the **Candidate** stage of the [project lifecycle](../governance/project-lifecycle.md).

## Expected to join first

### NHS Number

Validate, normalise, format and generate NHS Numbers (including the Scottish CHI and Northern Irish H&C ranges), with region checks. There are two implementations:

- **Python:** the `nhs-number` package. [Documentation](https://uk-fci.github.io/nhs-number/) · [Source](https://github.com/uk-fci/nhs-number)
- **Rust:** the `nhs-number` crate, by Joel Parker Henderson. [Source](https://github.com/joelparkerhenderson/nhs-number-using-rust) · [crates.io](https://crates.io/crates/nhs-number)

A shared, language-agnostic set of test vectors lets each implementation, and any future port, prove it gives the same answers.

### sct

A local-first SNOMED CT toolchain. One binary takes a raw RF2 release and turns it into NDJSON, SQLite, Parquet, Markdown, refsets and codelists, with fast local queries and tool use for LLMs, without depending on a terminology server.

[Documentation](https://pacharanero.github.io/sct/) · [Source](https://github.com/pacharanero/sct)

### clincalc

Open, community-auditable clinical calculators. A single Rust engine computes every score, and every surface (command line, Python package, MCP tool, REST API, desktop and web interfaces) is driven from it, so a result is identical wherever it appears. Each calculator cites primary literature, is tested against published vectors and records its licence.

[Documentation](https://pacharanero.github.io/clincalc/) · [Source](https://github.com/pacharanero/clincalc)

### GitEHR

A Git-based, decentralised, multi-contributor electronic health record. Clinical history is stored as files in a Git repository, inheriting Git's audit trail, integrity checks and offline working.

[Website](https://gitehr.org/) · [Source](https://github.com/gitehr/gitehr)

### anarchie

A complete openEHR clinical data repository, written in Rust, that uses Git-tracked flat files instead of a database server for persistence.

[Documentation](https://pacharanero.github.io/anarchie/) · [Source](https://github.com/pacharanero/anarchie)

## Other candidates

### Open Clinical Terminology (OCT)

An open clinical terminology, developed in the open.

[Website](http://openterminology.org/) · [Source](https://github.com/openterminology/oct)

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
