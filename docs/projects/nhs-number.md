---
description: NHS Number libraries for Python and JavaScript - validate, normalise and classify NHS and CHI numbers, with shared test vectors so every implementation gives the same answers.
---

# NHS Number

OHTF's NHS Number libraries validate and normalise NHS Numbers, including the Scottish CHI and Northern Irish H&C ranges, and check which region a number belongs to. There are two packages, which give the same answers because both are tested against one shared set of test vectors.

**Python:** the `nhs-number` package on PyPI, which also formats numbers and generates synthetic ones for testing.

[PyPI](https://pypi.org/project/nhs-number/){ .md-button .md-button--primary } [Documentation](https://ohtf.github.io/nhs-number-py/){ .md-button } [Source](https://github.com/ohtf/nhs-number-py){ .md-button }

**JavaScript and TypeScript:** the `@ohtf/nhs-number-js` package on npm, for browser and Node.js applications.

[npm](https://www.npmjs.com/package/@ohtf/nhs-number-js){ .md-button .md-button--primary } [Source](https://github.com/ohtf/nhs-number-js){ .md-button }

## Why it matters

The NHS Number is how health and care services in England, Wales and the Isle of Man identify a patient, and related ranges do the same in Scotland and Northern Ireland. Almost every piece of NHS software handles one. A wrongly validated or mistyped number can attach information to the wrong person, so the rules for checking one should be implemented once, correctly, and shared.

- **One well-tested implementation per language** instead of the same checksum and range rules rewritten in every product.
- **Shared test vectors.** A language-agnostic file of test cases records exactly how the libraries behave. The JavaScript package runs the Python library's vectors unmodified, and a port in any other language can prove it gives the same answers in the same way. The [Rust implementation](candidates.md#nhs-number-for-rust) is another such port.
- **Scottish CHI numbers handled properly.** Both libraries check the date encoded in a CHI number and accept the Modulus 10 check digit some CHI numbers use, cases that some other validators miss.
- **Synthetic numbers for testing.** The Python package can generate valid numbers from ranges set aside for testing, so developers never need to use a real patient's number.

The Python library was previously hosted by the Faculty of Clinical Informatics. When the Faculty closed, it moved to OHTF, which is part of [why OHTF exists](../about/index.md#origins).

## In action

Python:

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

JavaScript, after `npm install @ohtf/nhs-number-js`:

```js
import { isValid, regionOf, standardiseFormat } from '@ohtf/nhs-number-js';

isValid('943 476 5919');        // true
isValid('1234567890');          // false
regionOf('943 476 5919');       // 'SYNTHETIC'
standardiseFormat('943-476-5919'); // '9434765919'
```

Output from version 0.1.0, installed from npm.

## Key facts

### Python

| | |
| --- | --- |
| Lifecycle status | Foundation Project, [Incubating](../governance/project-lifecycle.md) |
| Current version | 3.0.0, published on [PyPI](https://pypi.org/project/nhs-number/) |
| Runs on | Python 3.10 and later |
| Licence | MIT. Use it freely; no permission needed. |
| Authors | Andy Law and Marcus Baw |
| Clinical Safety Officer | Not applicable to the library on its own; systems that use it assess it within their own clinical safety case |
| Medical device | No assessment recorded. It checks and formats identifiers and makes no clinical calculation or recommendation. |
| Clinical safety documentation | None; the published test vectors are the evidence of its behaviour |
| Package | [`nhs-number` on PyPI](https://pypi.org/project/nhs-number/) |
| Source | [github.com/ohtf/nhs-number-py](https://github.com/ohtf/nhs-number-py) |
| Documentation | [ohtf.github.io/nhs-number-py](https://ohtf.github.io/nhs-number-py/) |

### JavaScript and TypeScript

| | |
| --- | --- |
| Lifecycle status | Part of the same Foundation Project, [Incubating](../governance/project-lifecycle.md) |
| Current version | 0.1.0, published on [npm](https://www.npmjs.com/package/@ohtf/nhs-number-js) as `@ohtf/nhs-number-js`. Early development, so its interface may still change. |
| Runs on | Node.js 22.13 and later, and browsers through a bundler. No runtime dependencies. |
| Licence | MIT for code; documentation CC BY-SA 4.0 |
| Authors | Marcus Baw, building on the Python library |
| Clinical Safety Officer | Not applicable to the library on its own; systems that use it assess it within their own clinical safety case |
| Medical device | Preliminary assessment: standalone format and checksum validation has no diagnostic or therapeutic purpose. Not yet signed off. |
| Clinical safety documentation | [`SAFETY.md`](https://github.com/ohtf/nhs-number-js/blob/main/SAFETY.md), with its hazards and mitigations. Not approved for live patient workflows. |
| Package | [`@ohtf/nhs-number-js` on npm](https://www.npmjs.com/package/@ohtf/nhs-number-js) |
| Source | [github.com/ohtf/nhs-number-js](https://github.com/ohtf/nhs-number-js) |
| Documentation | The repository [README](https://github.com/ohtf/nhs-number-js#readme) and [validation contract](https://github.com/ohtf/nhs-number-js/blob/main/spec/standard.md) |

Validating an NHS Number checks its format, check digit and range. It does not confirm that the number was issued or that it belongs to the patient in front of you.

Why is all this public? See [why we publish so much](../transparency/why-we-publish.md).

## Core team

The people who look after this project day to day:

- [Andy Law](../about/advisers.md)
- [Dr Marcus Baw](../about/advisers.md)

## Get involved

Report problems or suggest improvements as issues on the [Python](https://github.com/ohtf/nhs-number-py/issues) or [JavaScript](https://github.com/ohtf/nhs-number-js/issues) repository. If you are implementing NHS Number handling in another language, the [guide for other languages](https://ohtf.github.io/nhs-number-py/other-languages/) explains how to use the shared test vectors.
