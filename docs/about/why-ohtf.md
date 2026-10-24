---
description: Why a new foundation for open-source health technology, and how OHTF relates to existing organisations.
---

# Why OHTF exists

The question we are asked most is a fair one: *why isn't this a job for an existing organisation?*

The short answer is that there are excellent organisations on every side of this space, and each one is built for a different job. None of them is designed to be a health-specific home for open-source clinical software: libraries, tools and services that implementers build on. OHTF is built for exactly that, and it works alongside the others rather than in competition with them.

## The landscape

| Organisation type | Examples | What they do well | Why it is not this job |
| --- | --- | --- | --- |
| General-purpose software foundations | Apache Software Foundation, Eclipse Foundation, Linux Foundation, CNCF | Proven governance and infrastructure for large open-source projects. | They can host a health project, but provide no health-specific identity, clinical safety awareness or peer group of related health projects. A health library hosted there has few related health projects around it. |
| Sector sub-foundations | Linux Foundation Public Health | A neutral home for public health authority software. | Hosting is scoped to public health authority deployments, which rules out general clinical libraries. |
| Standards development organisations | HL7, SNOMED International, openEHR | Specifications and terminologies the whole sector relies on. | They publish standards. They are not homes for independent software or its maintainers. |
| Health architecture and global goods initiatives | OpenHIE, Digital Square | Reference architectures for national health information exchange; curation and funding for global health software. | They describe and fund platforms, often for low- and middle-income settings. They do not host and maintain developer-facing software. |
| UK health informatics communities | Apperta Foundation, BCS Health and Care | Open standards advocacy and professional community. | Platform-focused or professional-body-shaped, rather than a neutral home that holds and maintains independent code. |
| Global and humanitarian health bodies | WHO, UN agencies | Policy, guidance and global health programmes. | Their mandate is global policy and programmes. Maintaining individual software projects is outside it. |

## What OHTF adds

1. **Developer-first.** OHTF looks after working code for implementers: the libraries you `pip install`, not the policy behind them.
2. **A neutral, health-specific home.** Projects get a peer group of related health software, without having to fit a general-purpose foundation's process, and without being left in a personal account.
3. **Health-specific governance.** Clinical safety documentation, careful handling of terminology and reference-data licensing, and contribution terms that make sense in health care.
4. **International scope.** UK-based and NHS-aware, but not tied to one country's national architecture.
5. **Low overhead.** A lean organisation with simple processes, so that joining does not cost a project more effort than it saves.

## Options we considered first

Starting a new organisation is a real cost, so we looked at lighter alternatives first:

- **A well-run GitHub organisation** with a charter, code of conduct and named maintainers gets most of the practical benefit at almost no cost. That is how OHTF started, and it is still the right first step for any new project.
- **An Eclipse Foundation working group**, which is designed for industry-specific clusters of projects. It did not meet OHTF's need to hold its own trademarks and to be a UK-credible neutral home for NHS-adjacent clinical safety governance.
- **Fiscal sponsorship**, for example through the Software Freedom Conservancy or Open Collective Europe. This lets a project take donations and hold assets inside someone else's organisation. It remains a good option for individual projects, but it does not make OHTF itself the neutral entity.

What tipped the balance towards incorporating: the need for a neutral holder of project trademarks, so that no single founder's company owns them; contributors whose employers want a clear, non-profit copyright holder; and the need for a durable organisation that clinical safety responsibilities can attach to.
