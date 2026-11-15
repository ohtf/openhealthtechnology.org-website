---
description: Awesome Missing NHS Things, the public list of what NHS and UK health and care work needs but doesn't have, where it came from, and how it led to OHTF.
---

# Awesome Missing NHS Things

[Awesome Missing NHS Things](https://ohtf.github.io/awesome-missing-nhs-things/) is a public list of the software, APIs, open data, components and infrastructure that NHS and UK health and care work needs but doesn't have. Several of OHTF's projects started as entries on it.

[Read the list](https://ohtf.github.io/awesome-missing-nhs-things/){ .md-button .md-button--primary } [Source](https://github.com/ohtf/awesome-missing-nhs-things){ .md-button }

## What it is

"Awesome lists" are a GitHub tradition: curated collections of the best tools on a subject. This one turns the idea round and records what is conspicuously absent, or what exists only under a licence, paywall or closed platform that stops anyone else building on it. Examples include an open ADHD assessment tool that services can embed, medicine shortage alerts at the moment of prescribing, and an API that says who is on call.

Every entry starts with a status (`missing`, `restricted`, `partial`, `building` or `solved`) and cites a source for each claim it makes. When a gap is filled, the entry stays on the list, marked `solved`, with a link to whoever filled it.

The list is for developers looking for something worth building, clinicians who keep running into the same gaps, and anyone deciding what to fund. It is not a Foundation Project, and it does not set OHTF policy. OHTF looks after it because it describes the problems OHTF exists to work on.

## Where it came from

Dr Marcus Baw, one of OHTF's founders, started the list in November 2018 in his own GitHub account, as a companion to [awesome-healthcare](https://github.com/kakoni/awesome-healthcare). The first version was a single line describing missing NHS and social care interfaces, services, registers and data sources, followed by a short list of national APIs and staff registers that ought to exist.

2019
:   Clinical calculation APIs went on the list in January, then an open platform for the statutory and mandatory training that NHS staff repeat every year.

2020
:   A larger round of additions in November covered organisation and location registers, health map layers and terminology.

2021
:   A communications section, written after the COVID pandemic showed that email to clinical staff depends on their link to a "home organisation", so sessional, locum and bank staff could not be reached. The first outside contributions arrived the same year, from Rob Dyke and HarvsG on GitHub; HarvsG added the point that a bleep represents a role, not a person.

2026
:   Entries began to record the open projects working on them. In November the list was rebuilt: every entry was re-checked against current sources and given a status, new sections were added, and the list moved to [github.com/ohtf](https://github.com/ohtf/awesome-missing-nhs-things) with its own site.

## How it led to OHTF

Several entries turned into working software. The clinical calculation entry led to the RCPCH Incubator's open clinical calculation APIs, most visibly the [RCPCH Digital Growth Charts API](https://growth.rcpch.ac.uk/), and later to [Digital PEWS](../projects/digital-pews.md) and [clincalc](../projects/clincalc.md), both now Foundation Projects. The codelists entry led to `sct`, and the patient-centred record entry to GitEHR, both [candidate projects](../projects/candidates.md). The entry on preserving NHS technical documentation led to rescued, searchable copies of specifications such as the NHS Common User Interface.

Building those projects exposed a gap the list had never named. Once open health software exists, it needs somewhere to live: a home that outlasts any one person's job, can hold its name and assets, and gives contributors' employers a clear answer about whose code it is. OHTF's [origins](index.md#origins) describe how that gap showed up in practice, and OHTF exists to fill it.

## What it means for OHTF

The list is a public backlog. Anyone can pick an entry and build it, and OHTF can give the result a neutral, long-term home: see [bring a project](../projects/bring-a-project.md).

Most entries need more than open-source code. National bodies, royal colleges, regulators or suppliers have to publish data, open up a licence or agree a standard, and the list records that progress whoever makes it.

## Contributing

Suggestions, corrections and news that something now exists are welcome. The list's [contributing guide](https://ohtf.github.io/awesome-missing-nhs-things/contributing/) explains what belongs on it and how to propose an entry.
