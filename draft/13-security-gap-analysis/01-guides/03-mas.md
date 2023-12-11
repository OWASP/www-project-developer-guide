---

title: Mobile Application Security
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 1311
permalink: /draft/security_gap_analysis/guides/mobile_application_security/

---

{% include breadcrumb.html %}

### 11.1.3 Mobile Application Security

The OWASP [Mobile Application Security][masproject] (MAS) flagship project has the mission statement:
"Define the industry standard for mobile application security".

The MAS project covers the processes, techniques, and tools used for security testing a mobile application,
as well as an exhaustive set of test cases that enables testers to deliver consistent and complete results.
The OWASP MAS project provides the [Mobile Application Security Verification Standard][masvs] (MASVS)
for mobile applications and a comprehensive [Mobile Application Security Testing Guide][mastg] (MASTG).

#### What is MASVS?

The OWASP MASVS is the industry standard for mobile app security.
It can be used by mobile software architects and developers seeking to develop secure mobile applications,
as well as security testers to ensure completeness and consistency of test results.

The MAS project has several uses; when it comes to security gap analysis then
the MASVS contains a list of security controls for mobile applications that are expected to be present / implemented.

The security controls are split into several categories:

* [MASVS-STORAGE](https://mas.owasp.org/MASVS/05-MASVS-STORAGE/)
* [MASVS-CRYPTO](https://mas.owasp.org/MASVS/06-MASVS-CRYPTO/)
* [MASVS-AUTH](https://mas.owasp.org/MASVS/07-MASVS-AUTH/)
* [MASVS-NETWORK](https://mas.owasp.org/MASVS/08-MASVS-NETWORK/)
* [MASVS-PLATFORM](https://mas.owasp.org/MASVS/09-MASVS-PLATFORM/)
* [MASVS-CODE](https://mas.owasp.org/MASVS/10-MASVS-CODE/)
* [MASVS-RESILIENCE](https://mas.owasp.org/MASVS/11-MASVS-RESILIENCE/)

#### Why use MASVS?

The OWASP MASVS provides a list of security controls that are expected in a mobile application.
If the application does not implement any of the controls then this could become a compliance issue,
given that MASVS is the industry standard for mobile applications, so any omissions need to be justified.

#### How to use MASVS

MASVS can be [accessed online][masvs] and the links followed for the security controls;
the mobile application can then be inspected for compliance with each control.
In addition MASVS can be downloaded as a PDF which can, for example, be used for evidence or compliance purposes.

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue130103] or [edit on GitHub][edit130103].

[edit130103]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/13-security-gap-analysis/01-guides/03-mas.md
[issue130103]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2013-security-gap-analysis/01-guides/03-mas
[masproject]: https://owasp.org/www-project-mobile-app-security/
[mastg]: https://mas.owasp.org/MASTG/
[masvs]: https://mas.owasp.org/MASVS/

\newpage
