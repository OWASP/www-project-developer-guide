---

title: Vulnerable Applications
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 9100
permalink: /release/training_education/vulnerable_applications/

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

### 7.1 Vulnerable Applications

Vulnerable applications are useful for the Training and Education activities
described in the SAMM [Training and Awareness][sammgegta] section,
which in turn is part of the SAMM [Education & Guidance][sammgeg] security practice
within the [Governance][sammg] business function.

The vulnerable applications provide a safe environment where various vulnerable targets can be attacked.
This provides practice in using various penetration tools available to a tester,
without the risk of attack traffic triggering intrusion detection systems.
The OWASP [Vulnerable Web Applications Directory Project][vwad] (VWAD) provides a comprehensive list of
available intentionally-vulnerable web applications:

* Vulnerable [mobile applications][vwad-mobile]
* [Offline][vwad-offline] vulnerable web applications
* [Containerized][vwad-containers] vulnerable web applications
* vulnerable web applications [available Online][vwad-online]

Sections:  

7.1 [Juice Shop](01-juice-shop.md)  
7.2 [WebGoat](02-webgoat.md)  
7.3 [PyGoat](03-pygoat.md)  
7.4 [Security Shepherd](04-security-shepherd.md)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0910] or [edit on GitHub][edit0910].

[edit0910]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/09-training-education/01-vulnerable-apps/toc.md
[issue0910]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2009-training-education/01-vulnerable-apps/00-toc
[sammg]: https://owaspsamm.org/model/governance/
[sammgeg]: https://owaspsamm.org/model/governance/education-and-guidance/
[sammgegta]: https://owaspsamm.org/model/governance/education-and-guidance/stream-a/
[vwad]: https://owasp.org/www-project-vulnerable-web-applications-directory/
[vwad-containers]: https://owasp.org/www-project-vulnerable-web-applications-directory/#div-container
[vwad-mobile]: https://owasp.org/www-project-vulnerable-web-applications-directory/#div-mobile
[vwad-online]: https://owasp.org/www-project-vulnerable-web-applications-directory/#div-online
[vwad-offline]: https://owasp.org/www-project-vulnerable-web-applications-directory/#div-offline
