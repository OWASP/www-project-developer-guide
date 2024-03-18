---

title: Mobile Application Security
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 506
permalink: /release/requirements/mobile_application_security/

---

{% include breadcrumb.html %}

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


[mas]: https://mas.owasp.org/
[masproject]: https://owasp.org/www-project-mobile-app-security/
[mastg]: https://mas.owasp.org/MASTG/
[masvs]: https://mas.owasp.org/MASVS/

\newpage
