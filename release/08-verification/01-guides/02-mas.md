---

title: Mobile Application Security
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 812
permalink: /release/verification/guides/mobile_application_security/

---

{% include breadcrumb.html %}

### 6.1.2 Mobile Application Security

The OWASP [Mobile Application Security][masproject] (MAS) flagship project has the mission statement:
"Define the industry standard for mobile application security".

The MAS project covers the processes, techniques, and tools used for security testing a mobile application,
as well as an exhaustive set of test cases that enables testers to deliver consistent and complete results.
The OWASP MAS project provides the [Mobile Application Security Verification Standard][masvs] (MASVS)
for mobile applications and a comprehensive [Mobile Application Security Testing Guide][mastg] (MASTG).

#### What is MASTG?

The OWASP [Mobile Application Security Testing Guide][mastg] is a comprehensive manual
for mobile application security testing and reverse engineering.
It describes the technical processes used for verifying the controls listed in the OWASP MASVS.

The MASTG provides several resources for testing the controls:

* Sections detailing the concepts and theory behind testing of both Android and iOS platforms
* Lists of [tests][mastgtests] for each section of the [MASVS][masvs]
* Descriptions of [techniques][mastgtechs] for Android or iOS used during testing
* Lists of generic [tools][mastgtools] and also ones specific for Android or iOS
* Reference [applications][mastgapps] that can be used as training material

#### Why use MASTG?

The OWASP MASVS is the industry standard for mobile application security,
and provides a list of security controls that are expected in a mobile application.
If the application does not implement these controls correctly then it could be vulnerable;
the MASTG tests that the application has the controls listed in the MASVS.

#### How to use MASTG

The OWASP Spotlight series provides an overview of using the MASTG:
'Project 13 - [OWASP Mobile Security Testing Guide (MSTG)][spotlight13]'.

The MASTG project contains a large number of resources that can be used during verification
and testing of mobile applications; pick and choose the resources that are applicable to specific application.

* Refer to the MASTG section on the concepts and theory to ensure good understanding of the testing process
* Select the [MASTG tests][mastgtests] that are applicable to the application and its platform OS
* Use the section on [MASTG techniques][mastgtechs] to run the selected tests correctly
* Become familiar with the range of [MASTG tools][mastgtools] available and select the ones that you need
* Use the [MAS Checklists][masc] to provide evidence of compliance

----

[masproject]: https://owasp.org/www-project-mobile-app-security/
[masc]: https://mas.owasp.org/checklists/
[mastg]: https://mas.owasp.org/MASTG/
[mastgapps]: https://mas.owasp.org/MASTG/apps/
[mastgtests]: https://mas.owasp.org/MASTG/tests/
[mastgtechs]: https://mas.owasp.org/MASTG/techniques/
[mastgtools]: https://mas.owasp.org/MASTG/tools/
[masvs]: https://mas.owasp.org/MASVS/
[spotlight13]: https://youtu.be/b07OQd5KSrs

\newpage
