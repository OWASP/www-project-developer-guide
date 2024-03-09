---

title: Verification
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 800
permalink: /draft/verification/

---

{% include breadcrumb.html %}

## 6. Verification

[Verification][sammv] is one of the business functions described by the [OWASP SAMM][samm].

Verification focuses on the processes and activities related to how an organization checks
and tests artifacts produced throughout software development.
This typically includes quality assurance work such as testing,
but it can also include other review and evaluation activities.

Verification activities should include:

* Architecture assessment, validation and mitigation
* Requirements-driven testing including security control verification and misuse/abuse testing
* Automated security testing and baselining
* Manual security testing and penetration testing

These activities are supported by:

* Security guides
* Test tools
* Test frameworks
* Vulnerability management
* Checklists

Sections:

6.1 [Guides](01-guides/toc.md)  
6.1.1 [Web Security Testing Guide](01-guides/01-wstg.md)  
6.1.2 [Mobile Application Security](01-guides/02-mas.md)  
6.1.3 [Application Security Verification Standard](01-guides/03-asvs.md)  
6.2 [Tools](02-tools/toc.md)  
6.2.1 [Zed Attack Proxy](02-tools/01-zap.md)  
6.2.2 [Code Pulse](02-tools/02-code-pulse.md)  
6.2.3 [Amass](02-tools/03-amass.md)  
6.2.4 [Offensive Web Testing Framework](02-tools/04-owtf.md)  
6.2.5 [Nettacker](02-tools/05-nettacker.md)  
6.2.6 [OWASP Secure Headers Project](02-tools/06-secure-headers.md)  
6.3 [Frameworks](03-frameworks/toc.md)  
6.3.1 [Glue](03-frameworks/01-glue.md)  
6.3.2 [secureCodeBox](03-frameworks/02-secure-codebox.md)  
6.4 [Vulnerability management](04-vulnerability-management/toc.md)  
6.4.1 [DefectDojo](04-vulnerability-management/01-defectdojo.md)  
6.5 [Do's and Don'ts](05-dos-donts/toc.md)  
6.5.1 [Secure environment](05-dos-donts/01-secure-environment.md)  
6.5.2 [System hardening](05-dos-donts/02-system-hardening.md)  
6.5.3 [Open Source software](05-dos-donts/03-open-source-software.md)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0800] or [edit on GitHub][edit0800].

[edit0800]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/08-verification/toc.md
[issue0800]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2008-verification/00-toc
[samm]: https://owaspsamm.org/about/
[sammv]: https://owaspsamm.org/model/verification/
