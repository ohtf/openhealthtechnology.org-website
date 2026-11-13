---
description: The nhs-number Python package - validate, normalise, format and generate NHS Numbers, with shared test vectors for ports to other languages.
---

# NHS Number (Python)

The `nhs-number` Python package validates, normalises, formats and generates NHS Numbers, including the Scottish CHI and Northern Irish H&C ranges, with checks for which region a number belongs to.

[Read the documentation](https://ohtf.github.io/nhs-number-py/){ .md-button .md-button--primary } [Source](https://github.com/ohtf/nhs-number-py){ .md-button } [PyPI](https://pypi.org/project/nhs-number/){ .md-button }

## Why it matters

The NHS Number is how health and care services in England, Wales and the Isle of Man identify a patient, and related ranges do the same in Scotland and Northern Ireland. Almost every piece of NHS software handles one. A wrongly validated or mistyped number can attach information to the wrong person, so the rules for checking one should be implemented once, correctly, and shared.

- **One well-tested implementation** instead of the same checksum and range rules rewritten in every product.
- **Shared test vectors.** A language-agnostic file of test cases records exactly how the library behaves, so a port in any other language can prove it gives the same answers. The [Rust implementation](index.md#nhs-number-for-rust) is one such port.
- **Synthetic numbers for testing.** It can generate valid numbers from ranges set aside for testing, so developers never need to use a real patient's number.

The library was previously hosted by the Faculty of Clinical Informatics. When the Faculty closed, it moved to OHTF, which is part of [why OHTF exists](../about/index.md#origins).

## In action

```pycon
>>> import nhs_number
>>> nhs_number.is_valid("943 476 5919")
True
>>> nhs_number.is_valid("1234567890")
False
>>> nhs_number.generate(for_region=nhs_number.REGION_SYNTHETIC, quantity=2)
['9151759349', '9255758268']
```

Output from version 3.0.0, installed from PyPI.

## Key facts

| | |
| --- | --- |
| Lifecycle status | Foundation Project, [Incubating](../governance/project-lifecycle.md) |
| Current version | 3.0.0, published on [PyPI](https://pypi.org/project/nhs-number/) |
| Supported Python | 3.10 and later |
| Licence | MIT. Use it freely; no permission needed. |
| Authors | Andy Law and Marcus Baw |
| Clinical Safety Officer | Not applicable to the library on its own; systems that use it assess it within their own clinical safety case |
| Medical device | No assessment recorded. It checks and formats identifiers and makes no clinical calculation or recommendation. |
| Clinical safety documentation | None; the published test vectors are the evidence of its behaviour |
| Source | [github.com/ohtf/nhs-number-py](https://github.com/ohtf/nhs-number-py) |
| Documentation | [ohtf.github.io/nhs-number-py](https://ohtf.github.io/nhs-number-py/) |

Why is all this public? See [why we publish so much](../transparency/why-we-publish.md).

## Core team

The people who look after this project day to day:

- [Andy Law](../about/advisers.md)
- [Dr Marcus Baw](../about/advisers.md)

## Get involved

Report problems or suggest improvements as [issues](https://github.com/ohtf/nhs-number-py/issues). If you are implementing NHS Number handling in another language, the [guide for other languages](https://ohtf.github.io/nhs-number-py/other-languages/) explains how to use the shared test vectors.
