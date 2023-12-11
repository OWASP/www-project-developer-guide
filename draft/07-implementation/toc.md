---

title: Implementation
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 700
permalink: /draft/implementation/

---

{% include breadcrumb.html %}

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

5.1 [Documentation](01-documentation/toc.md)  
5.1.1 [Top 10 Proactive Controls](01-documentation/01-proactive-controls.md)  
5.1.2 [Go Secure Coding Practices](01-documentation/02-go-scp.md)  
5.1.3 [Cheatsheet Series](01-documentation/03-cheatsheets.md)  
5.2 [Dependencies](02-dependencies/toc.md)  
5.2.1 [Dependency-Check](02-dependencies/01-dependency-check.md)  
5.2.2 [Dependency-Track](02-dependencies/02-dependency-track.md)  
5.2.3 [CycloneDX](02-dependencies/03-cyclonedx.md)  
5.3 [Secure Libraries](03-secure-libraries/toc.md)  
5.3.1 [Enterprise Security API library](03-secure-libraries/01-esapi.md)  
5.3.2 [CSRFGuard library](03-secure-libraries/02-csrf-guard.md)  
5.3.3 [OWASP Secure Headers Project](03-secure-libraries/03-secure-headers.md)  
5.4 [Implementation Do's and Don'ts](04-dos-donts/toc.md)  
5.4.1 [Container security](04-dos-donts/01-container-security.md)  
5.4.2 [Secure coding](04-dos-donts/02-secure-coding.md)  
5.4.3 [Cryptographic practices](04-dos-donts/03-cryptographic-practices.md)  
5.4.4 [Application spoofing](04-dos-donts/04-application-spoofing.md)  
5.4.5 [Content Security Policy (CSP)](04-dos-donts/05-content-security-policy.md)  
5.4.6 [Exception and error handling](04-dos-donts/06-exception-error-handling.md)  
5.4.7 [File management](04-dos-donts/07-file-management.md)  
5.4.8 [Memory management](04-dos-donts/08-memory-management.md)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0700] or [edit on GitHub][edit0700].

[edit0700]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/07-implementation/00-toc.md
[issue0700]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2007-implementation/00-toc
[sammm]: https://owaspsamm.org/model/
[sammi]: https://owaspsamm.org/model/implementation/
