---

title: Implementation Dependencies
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order:

---

{% include breadcrumb.html %}

## 5.2 Dependencies

Management of software dependencies is described by the SAMM [Software Dependencies][sammisbsd] activity,
which in turn is part of the SAMM [Secure Build][sammisb] security practice
within the [Implementation][sammi] business function.

It is important to record all dependencies used throughout the target production environment.
This record is often referred to as a Software Bill of Materials (SBOM).
An ideal SBOM provides information on each dependency so that it can be tracked:

* Where it is used or referenced
* Version used
* License
* Source information and repository
* Support and maintenance status of the dependency

Having an SBOM provides the ability to quickly find out which applications are affected by a particular CVE, for example.

Sections:

5.2.1 [Dependency-Check](#dependency-check)  
5.2.2 [Dependency-Track](#dependency-track)  
5.2.3 [CycloneDX](#cyclonedx)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing then [submit an issue][issue0720].

[issue0720]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2007-implementation/02-dependencies/00-toc
[sammi]: https://owaspsamm.org/model/implementation/
[sammisb]: https://owaspsamm.org/model/implementation/secure-build/
[sammisbsd]: https://owaspsamm.org/model/implementation/secure-build/stream-b/

\newpage
