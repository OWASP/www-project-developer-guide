---

title: Mobile Application Security
layout: col-document
tags: OWASP Developer Guide
contributors: Roxana Calderon, Jon Gadsden
document: OWASP Developer Guide
order: 53130
permalink: /release-es/security_gap_analysis/guides/mobile_application_security/

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

![MAS logo](../../../../assets/images/logos/mas.png "OWASP MAS"){: .image-right }

### 11.1.3 Mobile Application Security

The OWASP [Mobile Application Security][masproject] (MAS) flagship project has the mission statement:
"Define the industry standard for mobile application security".

The MAS project covers the processes, techniques, and tools used for security testing a mobile application,
as well as an exhaustive set of test cases that enables testers to deliver consistent and complete results.
The OWASP MAS project provides the [Mobile Application Security Verification Standard][masvs] (MASVS)
for mobile applications that can be used as a guide for security gap analysis.

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

The OWASP MASVS provides a list of industry-standard security controls for [secure mobile applications][csmas].
If the application does not implement any of the controls then this could become a compliance issue,
given that MASVS is the industry standard for mobile applications, so any omissions need to be justified.

#### How to use MASVS

The MASVS provides a list of expected security controls for mobile applications,
and this can be used to identify missing or inadequate controls during the gap analysis.
These controls can then be tested using the [MAS Testing Guide][mastg].

MASVS can be [accessed online][masvs] and the links followed for the security controls;
the mobile application can then be inspected for compliance with each control.
This provides a starting point for a security gap evaluation for any existing controls.

#### References

* OWASP [Mobile Application Security][mas] (MAS)
* MAS [project][masproject]
* MAS [Testing Guide][mastg] (MASTG)
* MAS [Verification Standard][masvs] (MASVS)
* OWASP [Mobile Application Security][csmas] cheat sheet

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue130103] or [edit on GitHub][edit130103].

[csmas]: https://cheatsheetseries.owasp.org/cheatsheets/Mobile_Application_Security_Cheat_Sheet
[edit130103]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/13-security-gap-analysis/01-guides/03-mas.md
[issue130103]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2013-security-gap-analysis/01-guides/03-mas
[mas]: https://mas.owasp.org/
[masproject]: https://owasp.org/www-project-mobile-app-security/
[mastg]: https://mas.owasp.org/MASTG/
[masvs]: https://mas.owasp.org/MASVS/

\newpage