---
description: How decisions are made in OHTF projects - do-ocracy with explicit structure, and why OHTF does not describe itself as a meritocracy.
---

# Do-ocracy

OHTF projects run as a **do-ocracy**: the people who do the work decide how it is done. If you want something to happen, you can start doing it, in the open, without waiting for permission.

OHTF deliberately does **not** describe itself as a *meritocracy*. This page explains the difference, the known weaknesses of do-ocracy, and the structure OHTF puts around it so that it stays fair.

!!! note "Draft"

    This page describes OHTF's intended way of working. It will be confirmed alongside OHTF's other governance policies.

## What do-ocracy means

Do-ocracy is a way of making decisions in which "those who take initiative to do work in a group are empowered to make decisions about what they do" ([CommunityRule](https://communityrule.info/modules/do-ocracy/)). It is common in volunteer communities, hackerspaces and open-source projects. Drupal contributors, for example, have long described their project's governance as a do-ocracy, based on the self-allocation of tasks ([David Rozas, via the P2P Foundation wiki](https://wiki.p2pfoundation.net/Do-ocracy)). It also runs through Cory Doctorow's novel [*Walkaway*](https://craphound.com/category/walkaway/) (2017), whose communities leave conventional society and organise around whoever turns up and does the work.

In practice it means:

- **Initiative is welcome.** You do not need to be appointed to fix a bug, write documentation or propose a feature.
- **Authority follows the work.** The person doing a piece of work makes the day-to-day decisions about it.
- **Objections must come with engagement.** If you disagree with how something is being done, say so publicly and with reasons, or offer to do it differently yourself. "I don't like it" is not a veto.

The Apache Software Foundation's [lazy consensus](https://community.apache.org/committers/lazyConsensus.html) is the closest formal cousin: state your intent publicly, wait a reasonable time for objections, and proceed if there are none. OHTF uses the same mechanism.

## Why not "meritocracy"?

"Meritocracy" sounds like a neutral description of letting the best work win. Its history and its effects are less flattering.

**The word started as a warning.** Sociologist Michael Young coined it in his 1958 satire *The Rise of the Meritocracy*, describing a dystopia in which a self-justifying elite believed it had earned its position. In 2001, watching politicians adopt the word as an aspiration, he wrote that the book "was a satire meant to be a warning (which needless to say has not been heeded)" ([Down with meritocracy, The Guardian](https://www.theguardian.com/politics/2001/jun/29/comment)).

**"Merit" in open source mostly measures free time and access.** Contributing unpaid work requires spare time, money, equipment, confidence and freedom from caring responsibilities, which are not evenly distributed. The idea of a meritocracy "presumes that everyone starts off and continues through with the same level of access to opportunity, time, and money, which is unfortunately not the case" ([Ashe Dryden, The Ethics of Unpaid Labor and the OSS Community, 2013](https://ashedryden.com/blog/the-ethics-of-unpaid-labor-and-the-oss-community)). Research found open-source development to be far more male-dominated than other forms of software production, and that the belief that code is separate from the social, summed up in the phrase "patches don't have gender", made the mechanisms of exclusion harder to address ([Dawn Nafus, 'Patches don't have gender': What is not open in open source software, *New Media & Society*, 2012](https://journals.sagepub.com/doi/abs/10.1177/1461444811422887)).

**Merit accumulates and rarely expires, so it favours incumbents.** Status earned early tends to persist long after the work that earned it. The Apache Way, one of the most carefully designed open-source governance models, states that merit "does not expire" ([The Apache Way](https://www.apache.org/theapacheway/)); Apache balances that with other safeguards, such as disallowing benevolent dictators. Projects without those safeguards can leave early arrivals in control indefinitely.

**It narrows what counts as valuable.** Measuring people by the quality of their code alone undervalues documentation, design, review, mentoring, project management and community care ([Coraline Ada Ehmke, The Dehumanizing Myth of the Meritocracy, *Model View Culture*, 2015](https://modelviewculture.com/pieces/the-dehumanizing-myth-of-the-meritocracy)). In health software, it would also undervalue clinical review and safety work, which OHTF cannot do without.

**It is a convenient justification for control.** "I've earned the right to decide" is how self-appointed leaders justify overriding everyone else, long after their own contributions have slowed. Because merit is claimed rather than conferred, it cannot easily be challenged.

## Do-ocracy and meritocracy compared

| | Meritocracy (as commonly practised) | Do-ocracy (as OHTF practises it) |
| --- | --- | --- |
| Where authority comes from | Accumulated reputation and status | Doing the specific piece of work in front of you |
| How long it lasts | Indefinitely, once earned | While you are doing the work, scoped to that work |
| What counts | Mostly code, judged by those already inside | Code, docs, review, clinical input, safety, triage, mentoring |
| How to challenge it | Hard: authority is claimed, not conferred | Do the work differently, or raise a public, reasoned objection |
| Who it favours | Early arrivals and people with the most spare time | Whoever turns up, provided structure keeps the field level (see below) |

## The weaknesses of do-ocracy, and what OHTF does about them

Do-ocracy is not automatically fair. Its own advocates list its failure modes: it can give those with the most free time the most authority, cause burnout when responsibilities are not shared, and lead to conflicting, uncoordinated efforts ([CommunityRule](https://communityrule.info/modules/do-ocracy/)).

The deeper risk was described in 1970 by Jo Freeman in [*The Tyranny of Structurelessness*](https://www.jofreeman.com/joreen/tyranny.htm): there is no such thing as a structureless group. Where rules are not written down, informal networks of friends take over, and "structurelessness becomes a way of masking power". A do-ocracy without explicit structure becomes a meritocracy by another name.

So OHTF pairs do-ocracy with Freeman's principles of explicit, accountable structure:

1. **Decisions happen in public.** Proposals, discussions and decisions are made in issues, pull requests and public discussions, not in private chats. If a decision was made elsewhere, it is written up publicly.
2. **Lazy consensus has a clock.** State your intent in public and allow at least 72 hours, longer around holidays or for significant changes, before treating silence as agreement. This gives people with day jobs, caring responsibilities and different time zones a fair chance to respond.
3. **Authority is scoped and current.** A maintainer's authority covers their project and lasts while they are actively maintaining it. Maintainers who step back become *emeritus*: honoured and listed, but no longer holding decision rights. Roles are reviewed regularly, and handing on responsibility is normal, not a failure.
4. **All contributions count.** Review, documentation, testing, triage, clinical review, safety documentation, design and mentoring are all "doing", and are credited as such.
5. **Make room for newcomers.** Projects label approachable work, explain how decisions are made, and share knowledge rather than hoarding it. Nobody should be indispensable.
6. **Objections need reasons and a route forward.** A blocking objection must be public, explain the concern, and ideally propose an alternative. Unresolved disagreements go to the project's maintainers, and then, as a last resort, to OHTF's directors.

## What do-ocracy does not decide

Some decisions carry legal, clinical or personal consequences and have named owners rather than being open to whoever acts first:

- **Clinical safety sign-off**, which follows the project's documented clinical safety process.
- **Security embargoes and vulnerability handling**, which follow the [security policy](../community/security.md).
- **Licensing, copyright and trademarks**, which follow the [open-source commitment](open-source-commitment.md) and OHTF policy.
- **Code of conduct enforcement**, which follows the [code of conduct](../community/code-of-conduct.md).
- **OHTF's legal decisions as a company**, which its directors take collectively under their statutory duties. No individual, however long-serving, can override that.

## Further reading

- Jo Freeman, [*The Tyranny of Structurelessness*](https://www.jofreeman.com/joreen/tyranny.htm) (1970-73). The essential warning about informal power in "leaderless" groups, with seven principles for democratic structure.
- CommunityRule, [Do-ocracy](https://communityrule.info/modules/do-ocracy/). A concise definition, with strengths, failure modes and related practices such as lazy consensus.
- Apache Software Foundation, [Lazy consensus](https://community.apache.org/committers/lazyConsensus.html) and [Decision making](https://community.apache.org/committers/decisionMaking.html). A practical, well-tested description of making decisions without waiting for permission.
- P2P Foundation wiki, [Do-ocracy](https://wiki.p2pfoundation.net/Do-ocracy). Background, including Drupal's use of the term.
- Michael Young, [Down with meritocracy](https://www.theguardian.com/politics/2001/jun/29/comment), *The Guardian* (2001). The coiner of the word on how it was misread.
- Ashe Dryden, [The Ethics of Unpaid Labor and the OSS Community](https://ashedryden.com/blog/the-ethics-of-unpaid-labor-and-the-oss-community) (2013). Who can afford to contribute unpaid work, and what that does to "merit".
- Dawn Nafus, ['Patches don't have gender': What is not open in open source software](https://journals.sagepub.com/doi/abs/10.1177/1461444811422887), *New Media & Society* 14(4), 2012. Research on how ideas of openness and code-only judgement hide exclusion.
- Cory Doctorow, [*Walkaway*](https://craphound.com/category/walkaway/) (Tor, 2017). A novel imagining whole communities organised on do-ocracy lines, and what happens when they collide with the old order.
- Coraline Ada Ehmke, [The Dehumanizing Myth of the Meritocracy](https://modelviewculture.com/pieces/the-dehumanizing-myth-of-the-meritocracy), *Model View Culture* (2015). Why judging people by code alone narrows what a community values.
