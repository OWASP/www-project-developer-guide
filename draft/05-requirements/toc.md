---

title: Requirements
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden, Andreas Happe
document: OWASP Developer Guide
order: 500
permalink: /draft/requirements/

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

## 3. Requirements

Security requirements also provide a foundation of vetted security functionality for an application.
Instead of creating a custom approach to security for every application,
standard security requirements allow developers to reuse the definition of security controls and best practices;
those same vetted security requirements provide solutions for security issues that have occurred in the past.

The importance of understanding key security requirements is described in the [Security Requirements][sammdsr]
practice that is part of the [Design][sammd] business function section within the OWASP [SAMM model][samm].
Ideally structured software security requirements are available within with a security a requirements framework,
and these are utilized by both developer teams and product teams.
In addition suppliers to the organization must meet security requirements;
build security into supplier agreements in order to ensure compliance with organizational security requirements.

In summary, security requirements exist to prevent the repeat of past security failures.

Sections:

3.1 [Requirements in practice](01-requirements.md)  
3.2 [Risk profile](02-risk.md)  
3.3 [OpenCRE](03-opencre.md)  
3.4 [SecurityRAT](04-security-rat.md)  
3.5 [Application Security Verification Standard](05-asvs.md)  
3.6 [Mobile Application Security](06-mas.md)  
3.7 [Security Knowledge Framework](07-skf.md)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0500] or [edit on GitHub][edit0500].

[edit0500]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/05-requirements/toc.md
[issue0500]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2005-requirements/00-toc
[samm]: https://owaspsamm.org/about/
[sammd]: https://owaspsamm.org/model/design/
[sammdsr]: https://owaspsamm.org/model/design/security-requirements/
