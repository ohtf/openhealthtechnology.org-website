---
description: Candidate Foundation Projects for the Open Health Technology Foundation.
---

# Projects

These are OHTF's **candidate** projects. They are real, public, open-source projects, mostly started by people involved in founding OHTF. Being listed here is not a claim that OHTF owns or already maintains a project. Each one becomes a Foundation Project only when it has named maintainers and has completed [onboarding](bring-a-project.md).

Every project page links to where the code lives today. When a project moves under OHTF, its repository transfers to [github.com/ohtf](https://github.com/ohtf), and the old address redirects.

!!! info "Lifecycle status"

    All projects below are currently at the **Candidate** stage of the [project lifecycle](../governance/project-lifecycle.md).

## Identifiers and terminology

### NHS Number

Validate, normalise, format and generate NHS Numbers (and the Scottish CHI and Northern Irish H&C ranges), with region checks. Includes a language-agnostic set of test vectors, so that ports in Rust and other languages can prove they agree with the reference implementation.

[Documentation](https://uk-fci.github.io/nhs-number/) · [Source](https://github.com/uk-fci/nhs-number) · Python package: `nhs-number`

### SNOMED CT tooling

`sct` is a local-first SNOMED CT toolchain: one binary that takes a raw RF2 release and turns it into NDJSON, SQL, Parquet, Markdown and fast local queries, without depending on a terminology server.

[Documentation](https://pacharanero.github.io/sct/) · [Source](https://github.com/pacharanero/sct)

### Open Clinical Terminology (OCT)

An open clinical terminology, developed in the open.

[Website](http://openterminology.org/) · [Source](https://github.com/openterminology/oct)

## Clinical logic

### Green Book

The UK childhood immunisation schedule (Green Book chapter 11) is published as PDFs, and every system that needs it re-implements it by hand. This project provides a computable, versioned schedule and an engine that evaluates a patient's FHIR vaccination history against it, with a shared conformance suite across implementations.

[Documentation](https://pacharanero.github.io/greenbook/) · [Source](https://github.com/pacharanero/greenbook)

## Records and documentation formats

### GitEHR

A Git-based, decentralised, multi-contributor electronic health record. Clinical history is stored as files in a Git repository, inheriting Git's audit trail, integrity checks and offline working.

[Website](https://gitehr.org/) · [Source](https://github.com/gitehr/gitehr)

### Medical Markdown

An early-stage specification, with reference parsers, for writing free-text clinical notes in a lightweight Markdown-like syntax that can be parsed into structured, coded data using standard clinical headings.

[Documentation](https://pacharanero.github.io/medical-markdown/) · [Source](https://github.com/pacharanero/medical-markdown)

### Archie

An openEHR clinical model processing and visualisation tool.

## Clinical safety

### SAFETY.md

A repository-native convention for clinical safety documentation. Like `README.md`, `LICENSE` and `SECURITY.md`, a root `SAFETY.md` puts the information reviewers, clinical safety officers and tools need where they will find it, next to the code, issues and releases that affect patient safety.

[Source](https://github.com/pacharanero/SAFETY.md)

## Publishing

### Clinicians Who Code: The Opinionated Handbook

A practical, opinionated guide for clinicians who want to build healthcare software safely, openly and quickly. Written by a clinician-developer, for clinician-developers.

[Read the handbook](https://pacharanero.github.io/clinicians-who-code-the-opinionated-handbook) · [Source](https://github.com/pacharanero/clinicians-who-code-the-opinionated-handbook)

## Not listed here?

If you maintain a small, reusable health technology component that needs a neutral, long-term home, see [bring a project](bring-a-project.md).
