---

title: Threat Modeling
layout: col-document
tags: Guia do Desenvolvedor do OWASP
contributors:
document: Guia do Desenvolvedor do OWASP
order: 26100
permalink: /release-pt-br/design/threat_modeling/

---

{% include breadcrumb.html %}

<style type="text/css">
.image-right {
  height: 180px;
  display: block;
  margin-left: auto;
  margin-right: auto;
  float: right;
}
</style>

![Developer guide logo](../../../assets/images/dg_logo_bbd.png "OWASP Developer Guide"){: .image-right }

### 4.1 Threat modeling

Referring to the [Threat Modeling Cheat Sheet][cstm],
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
4.1.2 [pytm](02-pytm.md)  
4.1.3 [Threat Dragon](03-threat-dragon.md)  
4.1.4 [Cornucopia](04-cornucopia.md)  
4.1.5 [LINDDUN GO](05-linddun-go.md)  
4.1.6 [Threat Modeling toolkit](06-toolkit.md)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0601] or [edit on GitHub][edit0601].

[edit0601]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/01-threat-modeling/toc.md
[issue0601]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/01-threat-modeling/00-toc
[cstm]: https://cheatsheetseries.owasp.org/cheatsheets/Threat_Modeling_Cheat_Sheet
