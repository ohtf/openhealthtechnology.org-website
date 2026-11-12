---
description: Digital PEWS, the open-source National Paediatric Early Warning System chart component, and OHTF's integration, training and support services for NHS organisations.
---

# Digital PEWS

Digital PEWS is an open-source charting and scoring component for the NHS National Paediatric Early Warning System (NPEWS) observation chart. It calculates NPEWS scores from observations recorded in your electronic patient record (EPR) and draws the chart clinicians recognise, inside the system they already use. Patient data stays in your EPR.

It is an OHTF Foundation Project. The work began at the Royal College of Paediatrics and Child Health (RCPCH); OHTF continues it independently following RCPCH's indefinite pause of its PEWS work, with existing attribution retained.

[Contact the Digital PEWS team](mailto:pews@openhealthtechnology.org?subject=Digital%20PEWS%20support){ .md-button .md-button--primary } [View the demo](https://ohtf.github.io/digital-pews/demo){ .md-button } [Source code](https://github.com/ohtf/digital-pews){ .md-button }

## How it works

- **A component, not a new system.** Digital PEWS is a bounded scoring and charting component. Your EPR keeps ownership of observation entry, patient identity, records, audit, alerts and escalation workflow.
- **EPR-agnostic.** It runs as a SMART on FHIR app, using the FHIR R4 standard to read observations from the host EPR, and can also be embedded directly in a web page or application.
- **Plain web technology.** Plain HTML, CSS and JavaScript, with no framework and no build step, so it is simple to host, review and maintain.
- **Open and auditable.** The source code is published under LGPL-3.0-or-later and the documentation and clinical content under CC BY-SA 4.0. Its scoring rules are defined in a machine-readable specification, traced to the NHS NPEWS source material and checked by automated tests.

## Support for NHS organisations

OHTF works with NHS trusts and other providers to take Digital PEWS from open-source component to a governed deployment in their own clinical system.

### Integration

Hands-on help connecting Digital PEWS to your EPR, including Oracle Health (Cerner Millennium) and other SMART on FHIR capable systems: app registration, launch configuration, FHIR mapping of your observation data, and testing against your environment, working alongside your EPR team and supplier.

### Clinical safety

Digital PEWS publishes its clinical safety documentation openly in the project's [`SAFETY.md`](https://github.com/ohtf/digital-pews/blob/main/SAFETY.md). OHTF provides the component's safety case material and works with your Clinical Safety Officer on your DCB0160 assessment of the integrated system. The component has no clinically approved release yet; completing that work for a deployment is part of what this service delivers.

### Training

Training for clinical, digital and EPR teams: how the chart and scores work, what the component does and does not do, configuration, and the safety controls your organisation owns.

### Ongoing support

An annual support agreement at a fixed price agreed in advance, so there are no surprise costs. It covers a named support contact, agreed response times, help with updates and new releases, and advice as the NPEWS specification and your EPR change.

### Open by default

Paid support never makes Digital PEWS less open. Improvements made during support work go back into the open project unless they are specific to your deployment, so every organisation using it benefits. See OHTF's [open-source commitment](../governance/open-source-commitment.md).

## Talk to us

To discuss integration, training or a support agreement for your organisation, email the Digital PEWS team at **[pews@openhealthtechnology.org](mailto:pews@openhealthtechnology.org?subject=Digital%20PEWS%20support)**.

[Contact the Digital PEWS team](mailto:pews@openhealthtechnology.org?subject=Digital%20PEWS%20support){ .md-button .md-button--primary }

To report a security vulnerability, use the [security policy](../community/security.md), not this address.
