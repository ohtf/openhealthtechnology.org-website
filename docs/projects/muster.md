---
description: Muster, an experimental open-source, LAN-first staff panic alarm for GP practices and other small workplaces.
---

# Muster

Muster is an open-source staff panic alarm for GP practices and other small workplaces. A member of staff presses and holds an on-screen button, and every other enrolled computer in the practice shows an alert and sounds an alarm. The person who raised the alarm sees, discreetly, that it was delivered and who is coming to help.

Muster is an experimental project: it is in early development and not yet suitable for use. "Muster" is a working name.

## Why it matters

Staff in GP practices sometimes face violence or aggression, and an on-screen panic alarm is often the quickest way to call colleagues. An alarm is only useful if it works when it is needed, and the person pressing it needs to know whether help is coming. Muster is designed around that:

- **It proves it works.** Every computer shows an honest status light, and must never claim to be connected when it cannot deliver an alarm. Scheduled drills produce coverage reports.
- **More than one way through.** Computers on the practice network find each other and deliver alarms directly, with an optional relay the practice can host itself to bridge separate networks and remote staff.
- **Silent to the room.** Raising an alarm makes no sound an aggressor would recognise.
- **Nothing leaves the practice.** No patient data, no telemetry and no third-party services. Messages are signed and encrypted, and the practice owns its keys and audit log.
- **Open.** Practices and their IT teams can inspect exactly how it works, and it runs on Windows, macOS and Linux.

## What it is not

- Not a monitored alarm service and not a route to 999. It alerts colleagues on site only; a practice's emergency procedures remain primary.
- Not a clinical system. It never handles patient data.

## Key facts

| | |
| --- | --- |
| Lifecycle status | [Experimental](../governance/project-lifecycle.md) |
| Maturity | Pre-alpha, under active development. Not yet suitable for use as a practice's panic alarm. |
| Licence | Code: AGPL-3.0-or-later, with an additional permission for app store distribution that is a draft pending legal review. Documentation: CC BY-SA 4.0. Alarm sounds: CC0. |
| Clinical Safety Officer | Not yet appointed. Required, with the project's release safety checks complete, before any practice uses it. |
| Medical device | Not a medical device. Recorded by Marcus Baw on 14 November 2026: Muster is a workplace staff-safety alarm with no medical purpose. The project still keeps a hazard log, because a failed alarm can harm staff. |
| Clinical safety documentation | Draft hazard log and safety case, kept in the project repository |
| Source | Not yet public |

Why is all this public? See [why we publish so much](../transparency/why-we-publish.md).

## Core team

The people who look after this project day to day:

- [Dr Marcus Baw](../about/advisers.md)
