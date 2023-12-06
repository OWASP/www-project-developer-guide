---

title: Operation
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order:

---

{% include breadcrumb.html %}

## 9. Operation

Operations are those activities necessary to ensure confidentiality, integrity, and availability are maintained
throughout the operational lifetime of an application and its associated data.
The aim of Operations is to provide greater assurance that the organization is resilient
in the face of operational disruptions, and responsive to changes in the operational landscape.
This is described by the OWASP SAMM model for the [Operations][sammo] business function.

Operations generally cover the security practices:

* [Incident Management][sammoim] of security breaches and incidents
* [Environment Management][sammoem] such as configuration hardening, patching and updating
* [Operational Management][sammoom] which includes data protection and system / legacy management

Sections:

9.1 [ModSecurity Core Rule Set](#modSecurity-core-rule-set)  
9.2 [Coraza Web Application Firewall](#coraza-web-application-firewall)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing then [submit an issue][issue1100].

[issue1100]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2011-operation/00-toc
[sammo]: https://owaspsamm.org/model/operations/
[sammoem]: https://owaspsamm.org/model/operations/environment-management/
[sammoim]: https://owaspsamm.org/model/operations/incident-management
[sammoom]: https://owaspsamm.org/model/operations/operational-management/

\newpage
