---

title: Verification Tools
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 820
permalink: /draft/verification/tools/

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

![Developer guide logo](../../../assets/images/dg_logo_bbd.png "OWASP Developer Guide"){: .image-right }

### 6.2 Verification tools

[Verification][sammv] is one of the business functions described by the [OWASP SAMM][samm].

The SAMM [Security Testing][sammvst] activity describes the use of both
automated security testing and manual expert security testing to discover security defects.
This security testing should be automated as part of the development, build and deployment processes;
and can be complemented with regular manual security penetration tests.

Automated security testing tools are fast and scale well to numerous applications,
whereas manual security testing of high-risk components requires good knowledge of the application and its business logic.

Sections:

6.2.1 [DAST](01-dast.md)  
6.2.2 [Amass](02-amass.md)  
6.2.3 [Offensive Web Testing Framework](03-owtf.md)  
6.2.4 [Nettacker](04-nettacker.md)  
6.2.5 [OWASP Secure Headers Project](05-secure-headers.md)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0820] or [edit on GitHub][edit0820].

[edit0820]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/08-verification/02-tools/toc.md
[issue0820]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2008-verification/02-tools/00-toc
[samm]: https://owaspsamm.org/about/
[sammv]: https://owaspsamm.org/model/verification/
[sammvst]: https://owaspsamm.org/model/verification/security-testing/
