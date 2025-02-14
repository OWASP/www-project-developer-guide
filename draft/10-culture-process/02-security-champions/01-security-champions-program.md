---

title: Security Champions Program
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 1021
permalink: /draft/culture_building_and_process_maturing/security_champions/program/

---

{% include breadcrumb.html %}

### 8.2.1 Security champions program

A Security Champion program is a commonly used way of helping development teams successfully run a development lifecycle
that is secure, and this is achieved by selecting members of teams to become Security Champions.
The role of Security Champion is described by the OWASP Software Assurance Maturity Model [(SAMM)][sammgegoc]
Organization and Culture activities within the Governance business function of the Education & Guidance practice.

#### Overview

The problem with development and security teams is their imbalance in numbers. There are usually less members in
the application security teams and thus a good way to scale and distribute security across the developement
teams is through a security champion role. The [Security Culture project][culturechamps] describes how this
can be implemented.

### Security champion role

The Security Champion is an individual of each developement team who shows special interest in application security.
They have knowledge and experience in both the aspects and hence can ensure that the development lifecycle has 
security built into it.

The general role for a security champion is to oversee threats and ensure secure coding practises are being
followed by their dev teams.

The [Security Culture project][culturechamps] provides a few more suggestions for what the role of a security champion
should look like. A few of these points are:

* Evangelize security: They **voice** for the best security practises in their team
* Contribute to standards: Provide inputs for the organization's security standards
* Engagement with security: Promote competitions such as Capture the Flag to instill
    security aspects into their teams (devs only learn when they break the apps they make)

#### Security champions program

The Security Champions program itself is to ensure that the right individuals are selected for the role and to
help them by providing support and training while also ensuring that they do not suffer from burn outs.
It is therefore important to select passionate individuals for this role.

For a successful program there are a few things an organisation needs to keep in mind:

* Passion towards security - identify the members of the teams that show interest in security
* Trust your champions - they are usually highly motivated when it comes to the security of their own applications
* Create a community - it can be lonely, so provide a support network to these individuals
* Have a clear vision - be pragmatic but ambitious, make it work, then make it work well

The OWASP [Security Champions Guide][scguide] identifies more principles that are important in this aspect
and will be a good read for an organisation that plans to go through this with this undertaking.

#### References

* OWASP [Security Champions Guide][scguide]
* [Security Champions Playbook][scplaybook]
* OWASP [Security Culture][culturedoc] project

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue1021] or [edit on GitHub][edit1021].

[edit1021]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/10-culture-process/02-security-champions/01-security-champions-program.md
[issue1021]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2010-culture-process/02-security-champions/01-security-champions-program
[sammgegoc]: https://owaspsamm.org/model/governance/education-and-guidance/stream-b/
[scguide]: https://owasp.org/www-project-security-champions-guidebook/
[scplaybook]: https://github.com/c0rdis/security-champions-playbook
[culturechamps]: https://owasp.org/www-project-security-culture/stable/4-Security_Champions/
[culturedoc]: https://owasp.org/www-project-security-culture/stable/

\newpage
