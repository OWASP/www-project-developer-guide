---

title: Threat modeling
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 503

---

{% include breadcrumb.html %}

### 5.3 Threat modeling

This section discusses Threat Modeling, an activity in the OWASP Software Assurance Maturity Model ([SAMM][samm]).
Threat modeling is part of the Threat Assessment security practice in the Design business function.
Much of the material in this section is drawn from the OWASP [Threat Model project][otm].

#### Overview

A threat model is essentially a structured representation of all the information
that affects the security of an application.
In essence, it is a view of the application and its environment through security glasses.

Threat modeling is a process for capturing, organizing, and analyzing all of this information.
and enables informed decision-making about application security risk.
In addition to producing a model, typical threat modeling efforts also produce a prioritized list
of _potential_ security vulnerabilities in the concept, requirements, design, or implementation.
Any potential vulnerabilities that have been identified from the model should then be remediated
using one of the common strategies: mitigate, eliminate, transfer or accept the threat of being exploited.

There are many reasons for doing threat modeling but the most important one is that this activity is _useful_ ,
it is probably the only stage in a development lifecycle where a team sits back and asks:
'If I was a very clever malicious actor with plenty of time, how would I subvert the application for my own purposes?'.
There are other reasons for threat modeling, for example standards compliance or analysis for disaster recovery,
but the main aim of threat modeling is to remedy potential vulnerabilities before the malicious actors do.

#### What is threat modeling

Threat modeling works to identify, communicate, and understand threats and mitigations
within the context of protecting something of value.

Threat modeling can be applied to a wide range of things, including software, applications, systems, networks,
distributed systems, things in the Internet of things, business processes, etc.
There are very few technical products which cannot be threat modeled;
more or less rewarding, depending on how much it communicates, or interacts, with the world.

The threat model is a record of the threat modeling process, and often includes:

* the description / design / model of what you’re worried about
* a list of assumptions that can be checked or challenged in the future as the threat landscape changes
* potential threats to the system
* remediation / actions to be taken for each threat
* ways of validating the model and threats, and verification of success of actions taken

The threat model should be in a form that can be easily revised and modified
during subsequent threat modeling discussions.

#### Why do it

Like all engineering activities, effort spent on threat modeling has to be justifiable.
Rarely any project or development has engineering effort that is going 'spare',
and the benefits of threat modeling have to outweigh the engineering cost of this activity.
Usually this is difficult to quantify; an easier way to approach it may be to ask
what are the costs of _not_ doing threat modeling?
These costs may consist of a lack of compliance, an increased risk of being exploited, harm to reputation and so on.

The inclusion of threat modeling in the secure development activities can help:

* Build a secure design
* Efficient investment of resources; appropriately prioritize security, development, and other tasks
* Bring Security and Development together to collaborate on a shared understanding, informing development of the system
* Identify threats and compliance requirements, and evaluate their risk
* Define and build required controls.
* Balance risks, controls, and usability
* Identify where building a control is unnecessary, based on acceptable risk
* Document threats and mitigation
* Ensure business requirements (or goals) are adequately protected in the face of
    a malicious actor, accidents, or other causes of impact
* Identification of security test cases / security test scenarios to test the security requirements

Threat modeling also provides a clear “line of sight” across a project that can be used
to justify other security efforts.
The threat model allows security decisions to be made rationally, with all the information available,
so that security decisions can be properly supported.
The threat modeling process naturally produces an assurance argument that can be used to explain
and defend the security of an application.
An assurance argument starts with a few high level claims and then justifies them with either sub-claims or evidence.

#### When to threat model

There is no wrong time to do threat modeling;
the earlier it is done in the development lifecycle the more beneficial it is,
but it threat modeling is also useful at any time during application development.

Threat modeling is best applied continuously throughout a software development project.
The process is essentially the same at different levels of abstraction,
although the information gets more and more granular throughout the development lifecycle.
Ideally, a high-level threat model should be defined in the concept or planning phase,
and then refined during the development phases.
As more details are added to the system new attack vectors are identified,
so the ongoing threat modeling process should examine, diagnose, and address these threats.

Note that it is a natural part of refining a system for new threats to be exposed.
For example, when you select a particular technology, such as Java for example,
you take on the responsibility to identify the new threats that are created by that choice.
Even implementation choices such as using regular expressions for validation
introduce potential new threats to deal with.

Threat modeling: _the sooner the better, but never too late_

#### Questions to ask

Often threat modeling is a conceptual activity rather than a rigorous process,
where development teams are brought together and asked to think up ways of subverting their system.
To provide some structure it is useful to start with Shostack's [Four Question Framework][4QFW]:

**1 What are we building**?

As a starting point you need to define the scope of the Threat Model.
To do that you need to understand the application you are building, examples of helpful techniques are:

* Architecture diagrams
* Dataflow transitions
* Data classifications

You will also need to gather people from different roles with sufficient technical and risk awareness
to agree on the framework to be used during the Threat modeling exercise.

**2 What can go wrong**?

This is a research activity in which you want to find the main threats that apply to your application.
There are many ways to approach the question, including open discussion or using a structure to help think it through.
Techniques that can help include [CIA][cia], [STRIDE][stride], [LINDDUN][linddun],
[cyber kill chains][chains], [PASTA][pasta], common attack patterns ([CAPEC][capec]) and others.

**3 What are we going to do about that**?

In this phase you turn your findings into specific actions.
Consider the appropriate [remediation](#remediation) for each threat identified.

**4 Did we do a good enough job**?

Finally, carry out a retrospective activity over the work you have done to check
quality, feasibility, progress, or planning.

The OWASP [Threat Modeling Playbook][OTMP] goes into these practicalities in more detail
and provides strategies for maintaining threat modeling within an organisation.

#### How to do it

There is no one process for threat modeling.
How it is done in practice will vary according to the organisation's culture,
according to what type of system / application is being modeled
and according to preferences of the development team itself.
The various techniques and concepts are discussed in the [Threat Modeling Cheat Sheet][OTMCS]
and can be summarised:

1. Terminology: try to use standard terms such as actors, trust boundaries, etc as this will help convey these concepts
2. Scope: be clear what is being modeled and keep within this scope
3. Document: decide which tools and what outputs are required to satisfy compliance, for example
4. Decompose: break the system being modeled into manageable pieces and identify your trust boundaries
5. Agents: identify who the actors are (malicious or otherwise) and what they can do
6. Categorise: prioritise the threats taking into account probability, impact and any other factors
7. Remediation: be sure to decide what to do about any threats identified, the whole reason for threat modeling

It is worth saying this again: there are many ways to do threat modeling,
all perfectly valid, so choose the right process that works for a specific team.

#### Final advice

Finally some advice on threat modeling.

**Make it incremental**:

Use [incremental threat modeling](https://owaspsamm.org/guidance/agile/#TA).
It is almost certainly a bad idea trying to fully model an existing application or system;
it can be very time consuming modeling a whole system,
and by the time such a model was completed then it would probably be out of date.
Instead incrementally model new features or enhancements as and when they are being developed.

Incremental threat modeling assumes that existing applications and features
have already been attacked over time and these real world vulnerabilities have been remediated.
It is the new features or new applications that pose a greater security risk;
if they are vulnerable then they will reduce the security of the existing application or system.
Concentrating on the new changes applies threat modeling effort at the place that it is needed most;
at the very least the changes should not make the security worse - and ideally the security should be better.

**Tools are secondary**:

It is good to standardise threat modeling tools across an organisation,
but also allow teams to choose how they record their threat models.
If one team decides to use Threat Dragon, for example, and another wants to use a drawing board,
then that is usually fine.
The discussions had during the threat modeling process are more important than the tool used,
although you might ask the team using the drawing board how they implement their change control.

**Brevity is paramount**:

It is very easy to create a threat model that looks a lot like a system diagram, with many components and data flows.
This makes for a convincing diagram, but it is not a model specific to the threat of exploits,
instead concentrate on the attack / threat surfaces
and be robust in consolidating multiple system components into one threat model component.
This will keep the number of components and dataflows manageable, and focuses the discussion on what matters most:
malicious actors (external or internal) trying to subvert your system.

**Choose your methodology**:

It is a good strategy to choose a threat categorisation methodology for the whole organisation
and then try and keep to it.
This could be [STRIDE][stride] or [LINDDUN][linddun], but if the [CIA][cia] triad gives enough granularity
then that is a perfectly good choice.

#### Further reading

* [Threat Modeling Manifesto](https://www.threatmodelingmanifesto.org/)
* OWASP [Threat Model project](https://owasp.org/www-project-threat-model/)
* OWASP [Threat Modeling Cheat Sheet][OTMCS]
* OWASP [Threat Modeling Playbook (OTMP)][OTMP]
* OWASP [Attack Surface Analysis Cheat Sheet][ASACS]
* OWASP community pages on [Threat Modeling][TM] and the [Threat Modeling Process][TMP]
* [The Four Question Framework For Threat Modeling](https://youtu.be/Yt0PhyEdZXU) 60 second video
* Lockheed's [Cyber Kill Chain][chains]
* VerSprite's Process for Attack Simulation and Threat Analysis ([PASTA][pasta])

#### Resources

* Shostack's [Four Question Framework][4QFW]
* OWASP [pytm][PYTM] Pythonic Threat Modeling tool
* OWASP [Threat Dragon][TD] threat modeling tool using dataflow diagrams
* [Threagile](https://threagile.io), an open source project that provides for Agile threat modeling
* Microsoft [Threat Modeling Tool][TMT], a widely used tool throughout the security community and free to download
* [threatspec](https://github.com/threatspec/threatspec), an open source tool based on comments inline with code
* Mitre's Common Attack Pattern Enumeration and Classification ([CAPEC][capec])
* NIST [Common Vulnerability Scoring System Calculator][nist-cvss]

----

The OWASP Developer Guide is a community effort; if you see something that needs changing
then [submit an issue][issue0502] or a [pull request][pr] .

[4QFW]: https://github.com/adamshostack/4QuestionFrame
[ASACS]: https://cheatsheetseries.owasp.org/cheatsheets/Attack_Surface_Analysis_Cheat_Sheet.html
[capec]: https://capec.mitre.org/
[chains]: https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html
[cia]: https://www.nccoe.nist.gov/publication/1800-25/VolA/index.html
[issue0502]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2005-security-requirements/02-threat-modeling
[linddun]: https://www.linddun.org/
[nist-cvss]: https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator
[otm]: https://owasp.org/www-project-threat-model/
[OTMCS]: https://cheatsheetseries.owasp.org/cheatsheets/Threat_Modeling_Cheat_Sheet.html
[OTMP]: https://owasp.org/www-project-threat-modeling-playbook/
[pasta]: https://versprite.com/blog/what-is-pasta-threat-modeling/
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls
[PYTM]: https://owasp.org/www-project-pytm/
[samm]: https://owaspsamm.org/about/
[stride]: https://en.wikipedia.org/wiki/STRIDE_%28security%29
[TD]: https://owasp.org/www-project-threat-dragon/
[TM]: https://owasp.org/www-community/Threat_Modeling
[TMP]: https://owasp.org/www-community/Threat_Modeling_Process
[TMT]: https://learn.microsoft.com/en-us/azure/security/develop/threat-modeling-tool

\newpage
