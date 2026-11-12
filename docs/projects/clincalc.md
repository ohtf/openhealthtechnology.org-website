---
description: clincalc - open, community-auditable clinical calculators from a single Rust engine, each citing primary literature and tested against published vectors.
---

# clincalc

`clincalc` provides open, community-auditable clinical calculators. A single Rust engine computes every score, and every way of using it (command line, Python package, MCP tool for AI assistants, REST API, desktop and web interfaces) is driven from that engine, so a result is identical wherever it appears.

[Read the documentation](https://ohtf.github.io/clincalc/){ .md-button .md-button--primary } [Source](https://github.com/ohtf/clincalc){ .md-button } [Calculator catalogue](https://ohtf.github.io/clincalc/calculators/){ .md-button }

## Why it matters

Clinical scores such as CURB-65, CHA₂DS₂-VASc or the Glasgow Coma Scale are rebuilt separately inside many different products. Each rebuild is a chance for a small error, an outdated threshold or an untraceable source, and a clinician has no easy way to tell which product got it right.

`clincalc` is a reference implementation instead:

- **Every calculator cites its primary literature**, so the source of each rule can be checked.
- **Every calculator is tested against published vectors**, worked examples taken from that literature.
- **Every calculator records the licence it is distributed under.** Scores that cannot be shipped because they are proprietary or licence-locked are listed with the reason, rather than left out silently.
- **One engine, many surfaces.** A score computed in a desktop app, a Python data pipeline or an AI assistant comes from the same code.

## In action

```pycon
>>> import clincalc
>>> r = clincalc.calculate("curb65", {"confusion": False, "urea_mmol_l": 8,
...     "respiratory_rate": 32, "systolic_bp": 85, "diastolic_bp": 55, "age": 72})
>>> r["result"]
4
>>> print(r["interpretation"])
Score 4: high severity (approx. 22% 30-day mortality for scores 3-5 in the Lim derivation group). Provide inpatient care and refer to critical care if appropriate (NICE NG250). At a score of 4-5, specifically assess for transfer to critical care (BTS 2009). Where bloods are unavailable, CRB-65 (the urea-free variant) can be used in primary care.
>>> print(r["reference"])
Lim WS, van der Eerden MM, Laing R, et al. Defining community acquired pneumonia severity on presentation to hospital: an international derivation and validation study. Thorax. 2003;58(5):377-382. Mortality groups from Figure 2; place-of-care guidance per NICE NG250, with critical-care transfer assessment per BTS 2009.
```

Output from version 0.5.0 of the Python package, installed from PyPI, using an illustrative example rather than patient data.

## Key facts

| | |
| --- | --- |
| Lifecycle status | Foundation Project, [Incubating](../governance/project-lifecycle.md) |
| Current version | 0.5.0 |
| Calculators | 144 registry entries: 130 available, 14 named but unavailable with the reason recorded |
| Intended use | Software development, research, education and evaluation. Not a finished medical device, and not to be used on its own to make decisions about an individual patient's care. |
| Licence | Code: AGPL-3.0-or-later, with QRISK3 and QFracture ports under LGPL-3.0-or-later. Clinical content: CC BY-SA 4.0. |
| Maintainer | Marcus Baw |
| Clinical Safety Officer | Not yet appointed; the draft safety case awaits CSO review |
| Medical device | The project's position is that published source code is not itself a medical device, and that regulatory obligations attach to whoever builds and supplies a ready-to-use instance for clinical use. This position is a draft for specialist legal review. |
| Clinical safety documentation | Draft [safety case and hazard log](https://github.com/ohtf/clincalc/tree/main/clinical-safety) and [regulatory assessment](https://github.com/ohtf/clincalc/tree/main/regulatory), published in the repository |
| Source | [github.com/ohtf/clincalc](https://github.com/ohtf/clincalc) |
| Documentation | [ohtf.github.io/clincalc](https://ohtf.github.io/clincalc/) |

Why is all this public? See [why we publish so much](../transparency/why-we-publish.md).

## Get involved

Clinicians reviewing a calculator's logic, references and test vectors is as valuable as code. Report problems or suggest new calculators as [issues](https://github.com/ohtf/clincalc/issues).
