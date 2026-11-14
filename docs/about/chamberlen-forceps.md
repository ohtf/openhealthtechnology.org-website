---
description: Why OHTF's logo is a pair of Chamberlen forceps - a historical warning about secrecy and single points of failure in health technology.
---

# Our logo: why we chose the Chamberlen forceps

![](../assets/ohtf-mark.svg){ .ohtf-logo-figure width="80" height="129" }

OHTF's logo is a pair of Chamberlen forceps. We chose them because their story is a warning we never want to repeat.

OHTF exists because health technology should not depend on one vendor, one employer or one person's private knowledge. The Chamberlen forceps are an unusually vivid historical warning about what can happen when a useful health technology is held as a secret.

The Chamberlen family kept their method for assisted delivery private for roughly a century, passing it through the family rather than enabling wider scrutiny, learning and improvement.[^dunn]

## A technique kept behind closed doors

The Chamberlens practised midwifery in seventeenth-century England. Their forceps could assist a delivery without the destructive hooks then used when a baby could not be delivered. Instead of publishing the instrument and its method, the family treated both as a commercial and professional secret.

Accounts describe elaborate concealment. The instruments were carried in a gilded chest. The person giving birth was blindfolded, and the delivery took place under blankets with only the Chamberlens present. The point was not merely to keep the physical forceps out of sight. It was to prevent anyone else understanding the method.[^birth]

In 1670, Hugh Chamberlen went to Paris intending to sell the secret to the French government. The demonstration failed. That episode is not evidence that every use of forceps was unsafe, but it is a stark example of the problem with opaque techniques: outsiders could neither examine the method beforehand nor independently test, teach or improve it afterwards.[^birth]

The original instruments were not identified publicly until the early nineteenth century, after being found hidden at the Chamberlen family's Essex home. By then, other forceps designs had begun to circulate and practitioners such as William Smellie had developed the instruments and their use further.[^birth]

## What the story shows

The Chamberlen story is not an argument against expertise or against paid clinical work. It is an argument against making public benefit depend on a private black box.

### Secrecy creates a single point of failure

When knowledge lives only with a family, a supplier or a small inner circle, its survival depends on their continued willingness and ability to provide it. A change of job, employer, funding model or commercial interest can remove a capability that patients and services rely on.

### Secrecy prevents scrutiny

Others cannot check hidden methods for defects, limits or harms. They cannot reproduce results, challenge unsupported claims, or train enough people to make a service resilient. In clinical technology, those are safety properties, not academic niceties.

### Openness lets useful work compound

Publishing an interface, a specification, source code and evidence does not make a system safe by itself. It gives maintainers, clinicians, implementers and independent reviewers something real to inspect, test, correct and improve. It also means that an organisation can support a project without becoming the only place it can be understood or used.

## What OHTF does differently

OHTF keeps Foundation Project code, build and deployment configuration, tests and documentation publicly reusable. We can provide paid hosting, implementation, support and training, but those services must fund maintenance rather than enclose the underlying infrastructure. See our [open-source commitment](../governance/open-source-commitment.md).

Openness is not a substitute for clinical safety, regulation, information governance or competent implementation. A public repository is not a safety case. OHTF requires each project to be honest about its lifecycle, intended use, maintainers, security route and clinical-safety position. See the [project lifecycle](../governance/project-lifecycle.md) and [how to bring a project to OHTF](../projects/bring-a-project.md).

The lesson of the Chamberlens is not that every health technology must be given away without support. It is that the knowledge and infrastructure on which care depends must not be trapped in a box that only one group can open.

!!! note "A note on the history"

    This is not a claim that forceps are simple, harmless, or a model for modern care. Their history includes trauma, contested professional power and men displacing women who had long practised midwifery. Nor is every detail certain: historians cannot establish which Chamberlen first made the instrument. The central fact, that the family kept the method private for roughly a century, is well established.[^dunn]

## Sources

[^dunn]: P Dunn, [*The Chamberlen family (1560-1728) and obstetric forceps*](https://pmc.ncbi.nlm.nih.gov/articles/PMC1721004/), *Archives of Disease in Childhood: Fetal and Neonatal Edition* 1999;81:F232-F234.

[^birth]: S Sheikh, I Ganesaratnam and H Jan, [*The birth of forceps*](https://pmc.ncbi.nlm.nih.gov/articles/PMC3704058/), *JRSM Short Reports* 2013;4(7). The [RCP Museum's Hugh Chamberlen biography](https://history.rcp.ac.uk/inspiring-physicians/hugh-chamberlen) gives useful primary-era quotations but notes that the underlying 1878 biography reflects the biases of its time.
