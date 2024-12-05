---

title: Implementation
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order:

---

{% include breadcrumb.html %}

![Developer guide logo](../../assets/images/dg_logo.png "OWASP Developer Guide"){height=180px}

## 5. Implementation

The [Implementation][sammi] business function is described by the OWASP [Software Assurance Maturity Model][sammm] (SAMM).
Implementation is focused on the processes and activities related to how an organization
builds and deploys software components and its related defects.
Implementation activities have the most impact on the daily life of developers,
and an important goal of Implementation is to ship reliably working software with minimum defects.

Implementation should include security practices such as :

* Secure Build
* Secure Deployment
* Defect Management

Implementation is where the application / system begins to take shape; source code is written and tests are created.
The implementation of the application follows a secure development lifecycle, with security built in from the start.

The implementation will use a secure method of source code control and storage to fulfil the design security requirements.
The development team will be referring to documentation advising them of best practices,
they will be using secure libraries wherever possible in addition to checking and tracking external dependencies.

Much of the skill of implementation comes from experience, and taking into account the Do's and Don'ts
of secure development is an important knowledge activity in itself.

Sections:

5.1 [Documentation](#documentation)  
5.1.1 [Top 10 Proactive Controls](#top-proactive-controls)  
5.1.2 [Go Secure Coding Practices](#go-secure-coding-practices)  
5.1.3 [Cheatsheet Series](#cheatsheet-series)  
5.2 [Dependencies](#dependencies)
5.2.1 [Dependency-Check](#dependency-check)  
5.2.2 [Dependency-Track](#dependency-track)  
5.2.3 [CycloneDX](#cyclonedx)  
5.3 [Secure Libraries](#secure-libraries)  
5.3.1 [Enterprise Security API library](#enterprise-security-api-library)  
5.3.2 [CSRFGuard library](#csrfguard-library)  
5.3.3 [OWASP Secure Headers Project](#owasp-secure-headers-project)  
5.4 [Mobile application weakness enumeration](#mobile-application-weakness-enumeration)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing then [submit an issue][issue0700].

[issue0700]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2007-implementation/00-toc
[sammm]: https://owaspsamm.org/model/
[sammi]: https://owaspsamm.org/model/implementation/
