---

title: Verification Tools
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 820
permalink: /release/verification/tools/

---

{% include breadcrumb.html %}

### 6.2 Verification tools

[Verification][sammv] is one of the business functions described by the [OWASP SAMM][samm].

The SAMM [Security Testing][sammvst] activity describes the use of both
automated security testing and manual expert security testing to discover security defects.
This security testing should be automated as part of the development, build and deployment processes;
and can be complemented with regular manual security penetration tests.

Automated security testing tools are fast and scale well to numerous applications,
whereas manual security testing of high-risk components requires good knowledge of the application and its business logic.

Sections:

6.2.1 [Zed Attack Proxy](01-zap.md)  
6.2.2 [Amass](02-amass.md)  
6.2.3 [Offensive Web Testing Framework](03-owtf.md)  
6.2.4 [Nettacker](04-nettacker.md)  
6.2.5 [OWASP Secure Headers Project](05-secure-headers.md)  

----

[samm]: https://owaspsamm.org/about/
[sammv]: https://owaspsamm.org/model/verification/
[sammvst]: https://owaspsamm.org/model/verification/security-testing/
