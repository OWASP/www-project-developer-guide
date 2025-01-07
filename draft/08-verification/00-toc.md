---

title: Verification
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order:

---

{% include breadcrumb.html %}

![Developer guide logo](../../assets/images/dg_logo.png "OWASP Developer Guide"){height=180px}

## 6. Verification

[Verification][sammv] is one of the business functions described by the [OWASP SAMM][samm].

Verification focuses on the processes and activities related to how an organization checks
and tests artifacts produced throughout software development.
This typically includes quality assurance work such as testing, and also includes other review and evaluation activities.

Verification activities should include:

* Architecture assessment, validation and mitigation
* Requirements-driven testing
* Security control verification and misuse/abuse testing
* Automated security testing and baselining
* Manual security testing and penetration testing

These activities are supported by:

* Security guides
* Test tools
* Test frameworks
* Vulnerability management
* Checklists

Verification is an activity central to the secure software development lifecycle.
Refer to the [Security Culture][culturetest] project section for the various types of security testing.

Sections:

6.1 [Guides](#verification-guides)  
6.1.1 [WSTG](#wstg)  
6.1.2 [MASTG](#mastg)  
6.1.3 [ASVS](#asvs)  
6.2 [Tools](#verification-tools)  
6.2.1 [DAST tools](#dast-tools)  
6.2.2 [Amass](#amass)  
6.2.3 [OWTF](#owtf)  
6.2.4 [Nettacker](#nettacker)  
6.2.5 [OSHP verification](#oshp-verification)  
6.3 [Frameworks](#verification-frameworks)  
6.3.1 [secureCodeBox](#securecodebox)  
6.4 [Vulnerability management](#verification-vulnerability-management)  
6.4.1 [DefectDojo](#defectdojo)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing then [submit an issue][issue0800].

[culturetest]: https://owasp.org/www-project-security-culture/stable/7-Security_Testing/
[issue0800]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2008-verification/00-toc
[samm]: https://owaspsamm.org/about/
[sammv]: https://owaspsamm.org/model/verification/

\newpage
