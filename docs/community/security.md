---
description: How to report a security vulnerability in an Open Health Technology Foundation project.
---

# Security policy

Health software handles sensitive data and can affect patient care, so we take security reports seriously and handle them privately.

## Reporting a vulnerability

**Do not report suspected vulnerabilities in public issues, discussions or pull requests.**

Report them privately, either:

- through GitHub's **private vulnerability reporting** on the affected repository (the *Security* tab, then *Report a vulnerability*); or
- by email to **[security@openhealthtechnology.org](mailto:security@openhealthtechnology.org)**.

Please include:

- a description of the issue and its likely impact;
- the affected project, versions or commit hashes;
- safe steps to reproduce it; and
- any mitigation you can suggest.

Remove credentials, and any patient-identifiable or other sensitive data, from your report.

We aim to acknowledge reports within 5 working days and to give a substantive response within 15 working days.

## Safety-relevant reports

If the issue could affect patient safety, clinical workflow or patient-identifiable data, say so clearly. We triage it as both a security finding and a potential clinical safety hazard.

## Scope

This policy covers projects under [github.com/ohtf](https://github.com/ohtf) and this website. A project may publish its own `SECURITY.md` with additional detail; where it does, that takes precedence for that project. Vulnerabilities in upstream dependencies should go to their maintainers, but please tell us privately if they affect an OHTF project.

## Disclosure

We use coordinated disclosure. Once a fix is available, we publish an advisory or release note and, if you agree, credit you for the report. Any temporary restriction on publishing source code during a fix follows the narrow rules in the [open-source commitment](../governance/open-source-commitment.md#narrow-exceptions).
