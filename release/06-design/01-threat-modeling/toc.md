---

title: Threat Modeling
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 6100
permalink: /release/design/threat_modeling/

---

{% include breadcrumb.html %}

### 4.1 Threat modeling

Referring to the [Threat Modeling Cheat Sheet][tmcs],
threat modeling is a structured approach to identifying and prioritizing potential threats to a system.
The threat modeling process includes determining the value that potential mitigations would have
in reducing or neutralizing these threats.

Assessing potential threats during the design phase of your project can save significant resources
if during a later phase of the project refactoring is required to include risk mitigations.
The outcomes from the threat modeling activities generally include:

* Documenting how data flows through a system to identify where the system might be attacked
* Identifying as many potential threats to the system as possible
* Suggesting security controls that may be put in place to reduce the likelihood or impact of a potential threat

Sections:

4.1.1 [Threat modeling in practice](01-threat-modeling.md)  
4.1.2 [Pythonic Threat Modeling](02-pytm.md)  
4.1.3 [Threat Dragon](03-threat-dragon.md)  
4.1.4 [Cornucopia](04-cornucopia.md)  
4.1.5 [LINDDUN GO](05-linddun-go.md)  
4.1.6 [Threat Modeling toolkit](06-toolkit.md)  

----

[tmcs]: https://cheatsheetseries.owasp.org/cheatsheets/Threat_Modeling_Cheat_Sheet.html
