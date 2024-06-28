---

title: Mobile Application Security
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 5060
permalink: /release/requirements/mobile_application_security/

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

![MAS logo](../../../assets/images/logos/mas.png "OWASP MAS"){: .image-right }

### 3.6 Mobile Application Security

The OWASP [Mobile Application Security][masproject] (MAS) flagship project has the mission statement:
"Define the industry standard for mobile application security".

The MAS project covers the processes, techniques, and tools used for security testing a mobile application,
as well as an exhaustive set of test cases that enables testers to deliver consistent and complete results.
The OWASP MAS project provides the [Mobile Application Security Verification Standard][masvs] (MASVS)
for mobile applications and a comprehensive [Mobile Application Security Testing Guide][mastg] (MASTG).

#### What is MASVS?

The [OWASP MASVS][mas] is used by mobile software architects and developers seeking to develop secure mobile applications,
as well as security testers to ensure completeness and consistency of test results.
The MAS project has several uses; when it comes to defining requirements then
the MASVS contains a list of security controls for mobile applications.

The security controls are split into several categories:

* [MASVS-STORAGE](https://mas.owasp.org/MASVS/05-MASVS-STORAGE/)
* [MASVS-CRYPTO](https://mas.owasp.org/MASVS/06-MASVS-CRYPTO/)
* [MASVS-AUTH](https://mas.owasp.org/MASVS/07-MASVS-AUTH/)
* [MASVS-NETWORK](https://mas.owasp.org/MASVS/08-MASVS-NETWORK/)
* [MASVS-PLATFORM](https://mas.owasp.org/MASVS/09-MASVS-PLATFORM/)
* [MASVS-CODE](https://mas.owasp.org/MASVS/10-MASVS-CODE/)
* [MASVS-RESILIENCE](https://mas.owasp.org/MASVS/11-MASVS-RESILIENCE/)

#### Why use MASVS?

The OWASP MASVS is the industry standard for mobile application security
and it is expected that any given set of security requirements will satisfy the MASVS.
When defining security requirements for mobile applications then each security control in the MASVS should be considered.

#### How to use MASVS

MASVS can be [accessed online][masvs] and the links followed for each security control.
In addition MASVS can be downloaded as a PDF which can, for example, be used for evidence or compliance purposes.
Inspect each control within MASVS and regard it as a potential security requirement.

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0506] or [edit on GitHub][edit0506].

[edit0506]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/05-requirements/06-mas.md
[issue0506]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2005-requirements/06-mas
[mas]: https://mas.owasp.org/
[masproject]: https://owasp.org/www-project-mobile-app-security/
[mastg]: https://mas.owasp.org/MASTG/
[masvs]: https://mas.owasp.org/MASVS/
