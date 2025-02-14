---

title: Threat Modeling in Practice
layout: col-document
tags: OWASP Developer Guide
contributors: Adam Shostack, Jon Gadsden
document: OWASP Developer Guide
order: 611
permalink: /draft/design/threat_modeling/practical_threat_modeling/

---

{% include breadcrumb.html %}

### 4.1.1 Threat modeling in practice

This section discusses Threat Modeling, an activity described in the OWASP Software Assurance Maturity Model ([SAMM][samm]).
Threat modeling is part of the [Threat Assessment][sammdta] security practice in the [Design][sammd] business function.

Much of the material in this section is drawn from the OWASP [Threat Model project][tmproject],
and the philosophy of this section tries to follow the [Threat Modeling Manifesto][tmmanifesto].

![TMM logo](../../../../assets/images/logos/tmmanifesto.png "OWASP TM Manifesto"){: height="60px" }

#### Overview

Zero-day attacks can be extremely harmful, and we don't want developers to be in the blind side of things when it
comes to security of the ideas they implement. This is why teams are encouraged to use threat modeling practices.

These practices try to discover what can go wrong with a system and help determine what to do about it.
It helps teams make system models and diagrams, give thought to potential threats and mitigations and more.
A good overview of this activity is given in the [Security Culture][culturetm] project section on threat modeling.

The documentation below is a small introduction to the idea aimed at developers who are trying this out for the
first time. For a more detailed approach to threat modeling, you can read the [Threat modeling cheat sheet][cstm]
by owasp.

#### What is threat modeling

Threat modeling stands as a procedural guideline to ensuring security of a teams output.

It can be applied to software, applications, systems, networks, distributed systems,
Internet of things implementations, business processes, and more.

The goal is to create a record that includes:

* a description / design / model of what you’re worried about
* a list of assumptions that can be checked or challenged in the future as the threat landscape changes
* potential threats to the system
* remediation / actions to be taken for each threat
* ways of validating the model and threats, and verification of success of actions taken

#### Why do it

The efforts spent on threat modeling is justified when we consider the alternative,
that is _no threat modeling_. Products where this due diligence has not been implemented,
are at a blind risk of attacks.

The inclusion of threat modeling in the secure development activities can help:

* Bring Security and Development together
* Identify threats and compliance requirements, and evaluate their risk
* Ensure business requirements (or goals) are adequately protected in the face of
    a malicious actor, accidents, or other causes of impact

[This blog][tmimp] by Bridewell on the subject justifies this to an
enterprise level (if risk mitigation wasn't enough!)

#### When to threat model

It is beneficial to perform this analysis at anytime during development. It is best applied continuously
throughout a software development project.
This is a dynamic procedure and with more features added to the product, there are more risks involved.

For example, small things like introducing regex for user input introduces bypass strings!

#### Questions to ask

Threat modeling is more conceptual, with development teams coming together and thinking of
ways of subverting their system.

To provide some structure it is useful to start with Shostack's [Four Question Framework][4QFW]
as described briefly below:

**1 What are we working on?'**?

The first step is to understand the application through architecture diagrams,
data flows, and classifications. This step is enhanced when people from different roles
can pitch in and give inputs.

The base must be understood perfectly before attempting to figure out vulnerabilities.

**2 What can go wrong**?

Then you must research potential risks. This can be done using frameworks like
[STRIDE][stride], [LINDDUN][linddun], and [CAPEC][capec].

OWASP provides a set of cards, [Cornucopia][corncards] to provide suggestions for general
vulnerabilities.
To make the process more fun, [Elevation of Privileges][eop] can be used or its OWASP version
[Snakes and Ladders][snakes].

**3 What are we going to do about that**?

Now these threats need to be addressed by either:

* transfer
* avoidance
* mitigation
* elimination

**4 Did we do a good enough job**?

Lastly, teams must review the process for quality, feasibility, and progress.
A good reference is the OWASP [Threat Modeling Playbook][tmpb] for long-term strategies.

#### How to do it

Threat modeling is not standardized and depends on how the organization exactly
wants to carry it out. However, a good set of procedures are defined in the
[Threat Modeling Cheat Sheet][cstm] which are summarized below:

* Define clear scopes and stick to them
* Fix on tools and outputs required early on
* Use standard terminology throughout the document
* Categorize the threat with respect to probability of occurrence
    and impact.
* Have a remediation planned for each threat.

#### Final advice

Some final words on threat modeling.

**Make it incremental**:

It is important to focus on new features and not entire systems. Consider using
[incremental threat modeling][sammgata] which allows for new features to be tested
as and when they're implemented.

This is recommended because modeling a full system can lead to missed threats while
also taking much more time.

**Tools are secondary**:

The discussion between teams and different development groups matters
more than tools. You must ensure flexibility in your organization with regards
to the tools used by different teams.

**Brevity is paramount**:

Make sure that your threat model is not so complex that people aren't able to
understand it! Because in such a case, its useless.

It is a good idea to keep models focused on threat surfaces, not complex system diagrams.

**Choose your methodology**:

It is a good strategy to choose a threat categorization methodology for the whole organization
and keep to it.
For example this could be [STRIDE][stride] or [LINDDUN][linddun], but if the CIA triad provides enough granularity
then that is also a perfectly good choice.

#### Further reading

* [Threat Modeling Manifesto][tmmanifesto]
* OWASP [Threat Model project][tmproject]
* OWASP [Threat Modeling Cheat Sheet][cstm]
* OWASP [Threat Modeling Playbook (OTMP)][tmpb]
* OWASP [Attack Surface Analysis Cheat Sheet][asacs]
* OWASP community pages on [Threat Modeling][TM] and the [Threat Modeling Process][TMP]
* [The Four Question Framework For Threat Modeling](https://youtu.be/Yt0PhyEdZXU) 60 second video
* Lockheed's [Cyber Kill Chain][chains]
* VerSprite's Process for Attack Simulation and Threat Analysis ([PASTA][pasta])
* [Threat Modeling: Designing for Security][TMdesigning]
* [Threat Modeling: A Practical Guide for Development Teams][TMpractical]

#### Resources

* Shostack's [Four Question Framework][4QFW]
* OWASP [pytm][PYTM] Pythonic Threat Modeling tool
* OWASP [Threat Dragon][tdtm] threat modeling tool using dataflow diagrams
* [Threagile](https://threagile.io), an open source project that provides for Agile threat modeling
* Microsoft [Threat Modeling Tool][TMT], a widely used tool throughout the security community and free to download
* [threatspec](https://github.com/threatspec/threatspec), an open source tool based on comments inline with code
* MITRE's Common Attack Pattern Enumeration and Classification ([CAPEC][capec])
* NIST [Common Vulnerability Scoring System Calculator][nist-cvss]
* OWASP [Network Segmentation Cheat Sheet][ccsnet]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue060101] or [edit on GitHub][edit060101].

[4QFW]: https://github.com/adamshostack/4QuestionFrame
[asacs]: https://cheatsheetseries.owasp.org/cheatsheets/Attack_Surface_Analysis_Cheat_Sheet
[capec]: https://capec.mitre.org/
[chains]: https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html
[corncards]: https://owasp.org/www-project-cornucopia/
[ccsnet]: https://cheatsheetseries.owasp.org/cheatsheets/Network_Segmentation_Cheat_Sheet
[cstm]: https://cheatsheetseries.owasp.org/cheatsheets/Threat_Modeling_Cheat_Sheet
[culturetm]: https://owasp.org/www-project-security-culture/stable/6-Threat_Modelling/
[eop]: https://shostack.org/games/elevation-of-privilege
[edit060101]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/01-threat-modeling/01-threat-modeling.md
[issue060101]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/01-threat-modeling/01-threat-modeling
[linddun]: https://linddun.org/
[nist-cvss]: https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator
[pasta]: https://versprite.com/blog/what-is-pasta-threat-modeling/
[PYTM]: https://owasp.org/www-project-pytm/
[samm]: https://owaspsamm.org/about/
[sammd]: https://owaspsamm.org/model/design/
[sammdta]: https://owaspsamm.org/model/design/threat-assessment/
[sammgata]: https://owaspsamm.org/guidance/agile/#TA
[snakes]: https://owasp.org/www-project-snakes-and-ladders/
[stride]: https://en.wikipedia.org/wiki/STRIDE_%28security%29
[tdtm]: https://owasp.org/www-project-threat-dragon/
[tmimp]: https://www.bridewell.com/insights/blogs/detail/what-is-threat-modelling-and-why-is-it-important
[tmpb]: https://owasp.org/www-project-threat-modeling-playbook/
[tmproject]: https://owasp.org/www-project-threat-model/
[tmmanifesto]: https://www.threatmodelingmanifesto.org/
[TM]: https://owasp.org/www-community/Threat_Modeling
[TMP]: https://owasp.org/www-community/Threat_Modeling_Process
[TMdesigning]: https://shostack.org/books/threat-modeling-book
[TMpractical]: https://threatmodeling.dev/
[TMT]: https://learn.microsoft.com/en-us/azure/security/develop/threat-modeling-tool

\newpage
