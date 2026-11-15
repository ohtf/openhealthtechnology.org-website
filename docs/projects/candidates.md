---
description: Candidate projects proposed for the Open Health Technology Foundation and going through onboarding.
---

# Candidate projects

Candidate projects are public, open-source projects proposed or invited to join OHTF and going through [onboarding](bring-a-project.md). Until they join, each is governed by its original home, linked below. When a project joins, its repository transfers to [github.com/ohtf](https://github.com/ohtf), the old address redirects, and it becomes a [Foundation Project](index.md). See the [project lifecycle](../governance/project-lifecycle.md).

### NHS Number for Rust

The `nhs-number` Rust crate, by Joel Parker Henderson, implements the same NHS Number checks and is tested against the same shared vectors.

[Source](https://github.com/joelparkerhenderson/nhs-number-using-rust) · [crates.io](https://crates.io/crates/nhs-number)

### sct

A local-first SNOMED CT toolchain. One binary takes a raw RF2 release and turns it into NDJSON, SQLite, Parquet, Markdown, refsets and codelists, with fast local queries and tool use for LLMs, without depending on a terminology server.

**Status:** Candidate. **Maintainer:** Marcus Baw. The project remains governed at its current repository; its local-first, open-source and clinically focused purpose is unchanged. Source code is licensed AGPL-3.0-or-later. SNOMED CT data remains separately licensed by SNOMED International; the software licence does not grant rights to redistribute that data.

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
