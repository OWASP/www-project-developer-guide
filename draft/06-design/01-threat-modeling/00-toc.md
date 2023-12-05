---

title: Threat Modeling
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order:

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

4.1.1 [Threat modeling in practice](#threat-modeling-in-practice)  
4.1.2 [Pythonic Threat Modeling](#pythonic-threat-modeling)  
4.1.3 [Threat Dragon](#threat-dragon)  
4.1.4 [Threat Modeling and Cornucopia](#cornucopia)  
4.1.5 [Threat Modeling toolkit](#threat-modeling-toolkit)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing then [submit an issue][issue0601].

[issue0601]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/01-threat-modeling/00-toc
[tmcs]: https://cheatsheetseries.owasp.org/cheatsheets/Threat_Modeling_Cheat_Sheet.html

\newpage
