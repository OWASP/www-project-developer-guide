---

title: Operation
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order:

---

{% include breadcrumb.html %}

## 9. Operations

Operations are those activities necessary to ensure that confidentiality, integrity, and availability
are maintained throughout the operational lifetime of an application and its associated data.
The aim of Operations is to provide greater assurance that the organization is resilient
in the face of operational disruptions, and responsive to changes in the operational landscape.
This is described by the [Operations][sammo] business function in the OWASP [SAMM model][samm].

Operations generally cover the security practices:

* [Incident Management][sammoim] of security breaches and incidents
* [Environment Management][sammoem] such as configuration hardening, patching and updating
* [Operational Management][sammoom] which includes data protection and system / legacy management

OWASP projects provide the Core Rule Set that is used for both Coraza and ModSecurity web application firewalls,
which are widely used for data and system management.

Sections:

9.1 [DevSecOps Guideline](#devsecops-guideline)  
9.2 [Coraza Web Application Firewall](#coraza-web-application-firewall)  
9.3 [ModSecurity Web Application Firewall](#modsecurity-web-application-firewall)  
9.4 [ModSecurity Core Rule Set](#modSecurity-core-rule-set)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing then [submit an issue][issue1100].

[issue1100]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2011-operations/00-toc
[samm]: https://owaspsamm.org/about/
[sammo]: https://owaspsamm.org/model/operations/
[sammoem]: https://owaspsamm.org/model/operations/environment-management/
[sammoim]: https://owaspsamm.org/model/operations/incident-management
[sammoom]: https://owaspsamm.org/model/operations/operational-management/

\newpage
