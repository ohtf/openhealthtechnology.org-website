---
description: Developer Certificate of Origin sign-off for contributions to Open Health Technology Foundation projects.
---

# Developer Certificate of Origin

Every contribution to an OHTF project is signed off under the **Developer Certificate of Origin (DCO)**. The DCO is a short statement that you have the right to submit your contribution under the project's open-source licence. It is the same mechanism used by the Linux kernel and many other projects.

There is no separate agreement to sign and no copyright assignment. You keep the copyright in your contribution and license it under the project's licence.

## How to sign off

Add a `Signed-off-by` line to each commit, using your real name and an email address you control:

```text
Signed-off-by: Ada Lovelace <ada@example.com>
```

Git adds this for you with the `-s` flag:

```sh
git commit -s -m "fix: reject NHS Numbers with a check digit of 10"
```

To sign off every commit automatically in a repository:

```sh
git config format.signOff true
```

If you forgot to sign off your most recent commit:

```sh
git commit --amend --signoff
```

OHTF repositories check for sign-off on pull requests.

## Why OHTF uses the DCO

It gives every project a clear, public record of where each contribution came from and on what terms. That matters to the organisations that rely on OHTF projects, and to contributors whose employers want to know the position is clean.

## The certificate

The text below is reproduced verbatim, as its licence requires.

```text
Developer Certificate of Origin
Version 1.1

Copyright (C) 2004, 2006 The Linux Foundation and its contributors.

Everyone is permitted to copy and distribute verbatim copies of this
license document, but changing it is not allowed.


Developer's Certificate of Origin 1.1

By making a contribution to this project, I certify that:

(a) The contribution was created in whole or in part by me and I
    have the right to submit it under the open source license
    indicated in the file; or

(b) The contribution is based upon previous work that, to the best
    of my knowledge, is covered under an appropriate open source
    license and I have the right under that license to submit that
    work with modifications, whether created in whole or in part
    by me, under the same open source license (unless I am
    permitted to submit under a different license), as indicated
    in the file; or

(c) The contribution was provided directly to me by some other
    person who certified (a), (b) or (c) and I have not modified
    it.

(d) I understand and agree that this project and the contribution
    are public and that a record of the contribution (including all
    personal information I submit with it, including my sign-off) is
    maintained indefinitely and may be redistributed consistent with
    this project or the open source license(s) involved.
```

Source: [developercertificate.org](https://developercertificate.org/).
