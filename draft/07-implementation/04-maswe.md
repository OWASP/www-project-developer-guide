---

title: MAS Weakness Enumeration
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 640
permalink: /draft/implementation/mas_weakness_enumeration/

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

![MAS checklist logo](../../../assets/images/logos/mas.png "OWASP MASWE"){: .image-right }

### 5.4 Mobile application weakness enumeration

The OWASP [Mobile Application Security][masproject] (MAS) flagship project provides
industry standards for mobile application security.

The OWASP MASWE project ...

#### What is the MASWE?

The MAS Weakness Enumeration ...

The MASWE is split out into weakness categories that match the MASVS verification categories:

* [MASVS-STORAGE](https://mas.owasp.org/MASWE/MASVS-STORAGE/MASWE-0001/) sensitive data storage
* [MASVS-CRYPTO](https://mas.owasp.org/MASWE/MASVS-CRYPTO/MASWE-0009/) cryptography best practices
* [MASVS-AUTH](https://mas.owasp.org/MASWE/MASVS-AUTH/MASWE-0028/) authentication and authorization mechanisms
* [MASVS-NETWORK](https://mas.owasp.org/MASWE/MASVS-NETWORK/MASWE-0047/) network communications
* [MASVS-PLATFORM](https://mas.owasp.org/MASWE/MASVS-PLATFORM/MASWE-0053/) interactions with the mobile platform
* [MASVS-CODE](https://mas.owasp.org/MASWE/MASVS-CODE/MASWE-0075/) platform and third-party software
* [MASVS-RESILIENCE](https://mas.owasp.org/MASWE/MASVS-RESILIENCE/MASWE-0089/) integrity and running on a trusted platform
* [MASVS-PRIVACY](https://mas.owasp.org/MASWE/MASVS-PRIVACY/MASWE-0108/) privacy of users, data and resources

#### Why use it?

#### How to use it

#### References

* Mobile Application Security ([MAS][masproject]) project
* MAS [Checklist][masc]
* MAS Testing Guide ([MASTG][mastg])
* MAS Verification Standard ([MASVS][masvs])
* MAS Testing Guide ([MASTG][mastg])

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0704] or [edit on GitHub][edit0704].

[edit0704]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/07-implementation/04-maswe.md
[issue0704]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/07-implementation/04-maswe
[masproject]: https://owasp.org/www-project-mobile-app-security/
[masc]: https://mas.owasp.org/checklists/
[mastg]: https://mas.owasp.org/MASTG/
[masvs]: https://mas.owasp.org/MASVS/

\newpage
