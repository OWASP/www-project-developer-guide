---

title: Operation
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 11000
permalink: /release/operation/

---

{% include breadcrumb.html %}

## 9. Operation

Operations are those activities necessary to ensure confidentiality, integrity, and availability are maintained
throughout the operational lifetime of an application and its associated data.
The aim of Operations is to provide greater assurance that the organization is resilient
in the face of operational disruptions, and responsive to changes in the operational landscape.
This is described by the OWASP [SAMM model][samm] for the [Operations][sammo] business function.

Operations generally cover the security practices:

* [Incident Management][sammoim] of security breaches and incidents
* [Environment Management][sammoem] such as configuration hardening, patching and updating
* [Operational Management][sammoom] which includes data protection and system / legacy management

OWASP provides the Core Rule Set that is used for both Coraza and ModSecurity web application firewalls,
which are important for data and system management..

Sections:

9.1 [ModSecurity Core Rule Set](01-modsecurity-crs.md)  
9.2 [Coraza Web Application Firewall](02-coraza.md)  
9.3 [ModSecurity Web Application Firewall](03-modsecurity.md)  

----

[samm]: https://owaspsamm.org/about/
[sammo]: https://owaspsamm.org/model/operations/
[sammoem]: https://owaspsamm.org/model/operations/environment-management/
[sammoim]: https://owaspsamm.org/model/operations/incident-management
[sammoom]: https://owaspsamm.org/model/operations/operational-management/
