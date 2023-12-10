---

title: Threat Modeling
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 610
permalink: /draft/design/threat-modeling/

---

{% include breadcrumb.html %}

## 4.1 Threat modeling

Referring to the [Threat Modeling Cheat Sheet][tmcs],
threat modeling is a structured approach of identifying and prioritizing potential threats to a system.
The threat modeling process includes determining the value that potential mitigations would have
in reducing or neutralizing these threats.

Assessing potential threats during the design phase of your project can save significant resources
that might be needed to refactor the project to include risk mitigations during a later phase of the project.
The outputs from the threat modeling activities generally include:

* Documenting how data flows through a system to identify where the system might be attacked
* Identifying as many potential threats to the system as possible
* Suggesting security controls that may be put in place to reduce the likelihood or impact of a potential threat

Sections:

4.1.1 [Threat modeling in practice](01-threat-modeling.md)  
4.1.2 [Pythonic Threat Modeling](02-pytm.md)  
4.1.3 [Threat Dragon](03-threat-dragon.md)  
4.1.4 [Threat Modeling and Cornucopia](04-cornucopia.md)  
4.1.5 [Threat Modeling toolkit](05-toolkit.md)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0601] or [edit on GitHub][edit0601].

[issue0601]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/01-threat-modeling/00-toc
[edit0601]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/01-threat-modeling/toc.md
[tmcs]: https://cheatsheetseries.owasp.org/cheatsheets/Threat_Modeling_Cheat_Sheet.html
