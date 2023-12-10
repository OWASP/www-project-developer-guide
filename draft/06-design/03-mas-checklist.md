---

title: Mobile Application Checklist
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 630
permalink: /draft/design/mas-checklist/

---

{% include breadcrumb.html %}

### 4.3 Mobile application checklist

The OWASP [Mobile Application Security][masproject] (MAS) flagship project has the mission statement:
"Define the industry standard for mobile application security".

The MAS project covers the processes, techniques, and tools used for security testing a mobile application,
as well as an exhaustive set of test cases that enables testers to deliver consistent and complete results.
The OWASP MAS project provides the [Mobile Application Security Verification Standard][masvs] (MASVS)
for mobile applications and a comprehensive [Mobile Application Security Testing Guide][mastg] (MASTG).

The [Mobile Application Security Checklist][masc] contains links to the MASTG test cases for each MASVS control.

#### What is MAS Checklist?

The MAS Checklist provides a checklist that keeps track of the MASTG test cases for each MASVS control,
and the checklist is split out into categories that match the MASVS categories:

* [MASVS-STORAGE](https://mas.owasp.org/checklists/MASVS-STORAGE/) sensitive data storage
* [MASVS-CRYPTO](https://mas.owasp.org/checklists/MASVS-CRYPTO/) cryptography best practices
* [MASVS-AUTH](https://mas.owasp.org/checklists/MASVS-AUTH/) authentication and authorization mechanisms
* [MASVS-NETWORK](https://mas.owasp.org/checklists/MASVS-NETWORK/) network communications
* [MASVS-PLATFORM](https://mas.owasp.org/checklists/MASVS-PLATFORM/) interactions with the mobile platform
* [MASVS-CODE](https://mas.owasp.org/checklists/MASVS-CODE/) platform and data entry points along with third-party software
* [MASVS-RESILIENCE](https://mas.owasp.org/checklists/MASVS-RESILIENCE/) integrity and running on a trusted platform

In addition to the web links there is a [downloadable spreadsheet][masxls].

#### Why use it?

If the MASTG is being applied to a mobile application then the MAS Checklist is a handy reference
that can also be used for compliance purposes.

#### How to use it

The [online version][masc] is useful to list the MASVS controls and which MASTG tests apply.
Follow the links to access the individual controls and tests.

The [spreadsheet download][masxls] allows the status of each test to be recorded,
with a separate sheet for each MASVS category.
This record of test results can be used as evidence for compliance purposes.

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0603] or [edit on GitHub][edit0603].

[edit0603]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/03-mas-checklist.md
[issue0603]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/03-mas-checklist
[masproject]: https://owasp.org/www-project-mobile-app-security/
[masxls]: https://github.com/OWASP/owasp-mastg/releases/latest/download/OWASP_MAS_Checklist.xlsx
[masc]: https://mas.owasp.org/checklists/
[mastg]: https://mas.owasp.org/MASTG/
[masvs]: https://mas.owasp.org/MASVS/

\newpage
