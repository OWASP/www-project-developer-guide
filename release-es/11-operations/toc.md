---

title: Operation
layout: col-document
tags: OWASP Developer Guide
contributors: Roxana Calderon, Jon Gadsden
document: OWASP Developer Guide
order: 51000
permalink: /release-es/operations/

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

![Developer guide logo](../../assets/images/dg_logo.png "OWASP Developer Guide"){: .image-right }

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

OWASP projects provide the CRS that is used for both Coraza and ModSecurity web application firewalls,
which are widely used for data and system management.

Sections:

9.1 [DevSecOps Guideline](01-devsecops.md)  
9.2 [Coraza Web Application Firewall](02-coraza.md)  
9.3 [ModSecurity Web Application Firewall](03-modsecurity.md)  
9.4 [OWASP CRS](04-crs.md)  

----

Traducción de versión [original en inglés][release1100].

[edit1100]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/11-operations/toc.md

[samm]: https://owaspsamm.org/about/
[sammo]: https://owaspsamm.org/model/operations/
[sammoem]: https://owaspsamm.org/model/operations/environment-management/
[sammoim]: https://owaspsamm.org/model/operations/incident-management
[sammoom]: https://owaspsamm.org/model/operations/operational-management/
