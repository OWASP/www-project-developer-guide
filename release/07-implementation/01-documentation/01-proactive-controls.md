---

title: Top 10 Proactive Controls
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 7110
permalink: /release/implementation/documentation/proactive_controls/

---

{% include breadcrumb.html %}

### 5.1.1 Top 10 Proactive Controls

The OWASP Top Ten Proactive Controls describes the most important controls and control categories
that security architects and development teams should consider in web application projects.
The [Proactive Controls project][proactive10] is an OWASP Lab documentation project and
the PDF can be downloaded for [various languages][proactive10-pdf].

#### What are the Top 10 Proactive Controls?

The OWASP Top Ten Proactive Controls 2018 is a list of security techniques that should be considered for web applications.
They are ordered by order of importance, with control number 1 being the most important:

* C1: [Define Security Requirements][control1]
* C2: [Leverage Security Frameworks and Libraries][control2]
* C3: [Secure Database Access][control3]
* C4: [Encode and Escape Data][control4]
* C5: [[Validate All Inputs][control5]
* C6: [Implement Digital Identity][control6]
* C7: [Enforce Access Controls][control7]
* C8: [Protect Data Everywhere][control8]
* C9: [Implement Security Logging and Monitoring][control9]
* C10: [Handle all Errors and Exceptions][control10]

#### Why use them?

The Proactive Controls are a well established list of security controls, first published in 2014
so considering these controls can be seen as best practice.

#### How to apply them

The OWASP Spotlight series provides an overview of how to use this documentation project:
'Project 8 - [Proactive Controls][spotlight08]'.

During development of a web application, consider using each security control
described in the sections of the Proactive Controls that are relevant to the application.

----

[control1]: https://owasp.org/www-project-proactive-controls/v3/en/c1-security-requirements
[control2]: https://owasp.org/www-project-proactive-controls/v3/en/c2-leverage-security-frameworks-libraries
[control3]: https://owasp.org/www-project-proactive-controls/v3/en/c3-secure-database
[control4]: https://owasp.org/www-project-proactive-controls/v3/en/c4-encode-escape-data
[control5]: https://owasp.org/www-project-proactive-controls/v3/en/c5-validate-inputs
[control6]: https://owasp.org/www-project-proactive-controls/v3/en/c6-digital-identity
[control7]: https://owasp.org/www-project-proactive-controls/v3/en/c7-enforce-access-controls
[control8]: https://owasp.org/www-project-proactive-controls/v3/en/c8-protect-data-everywhere
[control9]: https://owasp.org/www-project-proactive-controls/v3/en/c9-security-logging
[control10]: https://owasp.org/www-project-proactive-controls/v3/en/c10-errors-exceptions
[proactive10]: https://owasp.org/www-project-proactive-controls/
[proactive10-pdf]: https://github.com/OWASP/www-project-proactive-controls/tree/master/v3
[spotlight08]: https://youtu.be/HRtYDCWOSc0

