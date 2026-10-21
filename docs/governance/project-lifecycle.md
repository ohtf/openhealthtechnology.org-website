---
description: The lifecycle stages an OHTF Foundation Project moves through, from candidate to archived.
---

# Project lifecycle

Every OHTF project has an explicit lifecycle status, shown on the [projects page](../projects/index.md) and in the project's own README. The status tells users how much they can rely on a project today.

!!! note "Draft"

    This lifecycle is a working draft and will be confirmed in OHTF's project acceptance policy.

| Status | Meaning | What you can expect |
| --- | --- | --- |
| **Candidate** | Proposed or invited, not yet onboarded. | The project is still governed by its original home. |
| **Incubating** | Accepted and moving under OHTF. Maintainers named; governance files being adopted. | Usable, but interfaces and processes may still change. |
| **Active** | Fully onboarded and maintained. | Named maintainers, security contact, DCO on contributions, releases following the project's stated versioning. |
| **Maintenance** | Stable, receiving security and critical fixes only. | Safe to keep using; new features unlikely. |
| **Archived** | No longer maintained. | Repository read-only and still openly licensed. Use at your own risk, or ask to revive it. |

## Moving between stages

- **Candidate to incubating:** the project has been [proposed](../projects/bring-a-project.md), has at least one named maintainer, and the maintainers agree to OHTF's [open-source commitment](open-source-commitment.md).
- **Incubating to active:** the repository is under [github.com/ohtf](https://github.com/ohtf) and has an open licence, a README with its status, a [security contact](../community/security.md), [DCO](../community/dco.md) checks on contributions, and, if it could affect patient care, a documented clinical safety position.
- **Active to maintenance:** the maintainers decide the project is feature-complete or their capacity has reduced, and say so publicly.
- **Any stage to archived:** no maintainer remains, or the project has been superseded. OHTF looks for new maintainers before archiving anything people still depend on.

Archived projects can be revived by new maintainers through the same route as a new candidate.
