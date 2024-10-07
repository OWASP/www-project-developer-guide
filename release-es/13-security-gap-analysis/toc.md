---

title: Security Gap Analysis
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 1300
permalink: /release-es/security_gap_analysis/

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

## 11. Security gap analysis

A security gap analysis is an activity where the information security posture of an organization is assessed
and any shortfalls or operation gaps are identified.
This activity can also be combined with a security gap evaluation where the existing controls and processes
are assessed for effectiveness and relevance.
Security gap analysis is required to gain or maintain certification to a management system standard
such as [ISO 27001][iso27001] 'Information security, cybersecurity and privacy protection'.

The security gap analysis is often associated with Governance, Risk & Compliance activities,
where the compliance with a management system standard is periodically reviewed and updated.
Guides and tools are useful for these compliance activities and the OWASP projects [SAMM][samm],
[MASVS][masvs] and [ASVS][asvs] provide information and advice in meeting management system standards.

Sections:

11.1 [Guides](01-guides/toc.md)  
11.1.1 [Software Assurance Maturity Model](01-guides/01-samm.md)  
11.1.2 [Application Security Verification Standard](01-guides/02-asvs.md)  
11.1.3 [Mobile Application Security](01-guides/03-mas.md)  
11.2 [Bug Logging Tool](02-blt.md)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue1300] or [edit on GitHub][edit1300].

[asvs]: https://owasp.org/www-project-application-security-verification-standard/
[edit1300]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/13-security-gap-analysis/toc.md
[iso27001]: https://www.iso.org/standard/82875.html
[issue1300]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2013-security-gap-analysis/00-toc
[masvs]: https://mas.owasp.org/MASVS/
[samm]: https://owaspsamm.org/about/
