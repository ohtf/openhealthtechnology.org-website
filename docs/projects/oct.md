---
description: oct, the Open Clinical Terminology - an open, community-owned clinical terminology that anyone can use without licence fees or restrictions.
---

# `oct` - Open Clinical Terminology

`oct` is an open, community-owned clinical terminology: a shared set of identifiers and descriptions for clinical concepts, built in the open from contributions by clinicians, developers and others, and free for anyone to use, change and share.

[Read the documentation](https://openterminology.org/){ .md-button .md-button--primary } [Source](https://github.com/ohtf/oct){ .md-button } [Discussion](https://openhealthhub.org/c/oct/58){ .md-button }

## Why it matters

Every clinical record system needs a terminology, a common vocabulary that lets a diagnosis, a symptom or a procedure mean the same thing everywhere it is recorded. The terminologies health systems rely on today are not open and free to use without restrictions, which limits who can build with them and how.

`oct` is built to be:

- **Open and free.** Anyone can use, modify and redistribute the terminology, including commercially, with attribution.
- **Clinically relevant.** It focuses on the concepts clinicians actually record.
- **Clean-room.** Every concept comes from open contributions or from existing works with a compatible open licence, never from closed terminologies.
- **Durable.** An identifier, once assigned, always means the same concept and is never reused or deleted.
- **Separated by design.** `oct` defines identifiers and descriptions; hierarchies and relationships live in separate ontologies that reference `oct` identifiers. Trying to keep one permanent namespace and one perfect hierarchy at the same time has proven intractable for existing terminologies.

## In action

Each `oct` concept has a short, non-semantic identifier that is safe to speak aloud, type, and use in URLs and filenames, and a description in each supported language. This is a concept from the `oct` repository:

```text
Identifier:   r9j3jq
Description:  Delusions of grandeur   (en-GB)
```

## Key facts

| | |
| --- | --- |
| Lifecycle status | Foundation Project, [Incubating](../governance/project-lifecycle.md) |
| Maturity | Early. The identifier scheme and design principles are specified; the terminology content is at an early stage and not yet ready for use in clinical systems. |
| Licence | Software: Apache-2.0. Terminology content and documentation: CC BY 4.0. |
| Clinical Safety Officer | Not applicable at this stage; required before any clinical deployment of a system using `oct` |
| Medical device | No assessment recorded. A terminology is a vocabulary, not software with a medical purpose; any system that uses it carries its own obligations. |
| Clinical safety documentation | None yet |
| Source | [github.com/ohtf/oct](https://github.com/ohtf/oct) |
| Documentation | [openterminology.org](https://openterminology.org/) |
| Discussion | [`oct` on Open Health Hub](https://openhealthhub.org/c/oct/58) |

Why is all this public? See [why we publish so much](../transparency/why-we-publish.md).

## Core team

The people who look after this project day to day:

- [Dr Marcus Baw](../about/advisers.md)

## Get involved

Discussion happens in the [`oct` category on Open Health Hub](https://openhealthhub.org/c/oct/58). Proposed changes to the terminology are made as pull requests to the [repository](https://github.com/ohtf/oct), and design decisions are open for discussion as RFCs.
