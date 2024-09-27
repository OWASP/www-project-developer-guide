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

Sections:

6.1 [Guides](01-guides/toc.md)  
6.1.1 [Web Security Testing Guide](01-guides/01-wstg.md)  
6.1.2 [MAS Testing Guide](01-guides/02-mastg.md)  
6.1.3 [Application Security Verification Standard](01-guides/03-asvs.md)  
6.2 [Tools](02-tools/toc.md)  
6.2.1 [DAST](02-tools/01-dast.md)  
6.2.2 [Amass](02-tools/02-amass.md)  
6.2.3 [Offensive Web Testing Framework](02-tools/03-owtf.md)  
6.2.4 [Nettacker](02-tools/04-nettacker.md)  
6.2.5 [OWASP Secure Headers Project](02-tools/05-secure-headers.md)  
6.3 [Frameworks](03-frameworks/toc.md)  
6.3.1 [secureCodeBox](03-frameworks/01-secure-codebox.md)  
6.4 [Vulnerability management](04-vulnerability-management/toc.md)  
6.4.1 [DefectDojo](04-vulnerability-management/01-defectdojo.md)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0800] or [edit on GitHub][edit0800].

[edit0800]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/08-verification/toc.md
[issue0800]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2008-verification/00-toc
[samm]: https://owaspsamm.org/about/
[sammv]: https://owaspsamm.org/model/verification/
