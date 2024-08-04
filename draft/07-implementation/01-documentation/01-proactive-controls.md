---

title: Top 10 Proactive Controls
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 711
permalink: /draft/implementation/documentation/proactive_controls/

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

* C1: [Define Security Requirements][control1], ref [Cheat Sheets][cheatsheet-proactive-c1]
* C2: [Leverage Security Frameworks and Libraries][control2], ref [Cheat Sheets][cheatsheet-proactive-c2]
* C3: [Secure Database Access][control3], ref [Cheat Sheets][cheatsheet-proactive-c3]
* C4: [Encode and Escape Data][control4], ref [Cheat Sheets][cheatsheet-proactive-c4]
* C5: [Validate All Inputs][control5], ref [Cheat Sheets][cheatsheet-proactive-c5]
* C6: [Implement Digital Identity][control6], ref [Cheat Sheets][cheatsheet-proactive-c6]
* C7: [Enforce Access Controls][control7], ref [Cheat Sheets][cheatsheet-proactive-c7]
* C8: [Protect Data Everywhere][control8], ref [Cheat Sheets][cheatsheet-proactive-c8]
* C9: [Implement Security Logging and Monitoring][control9], ref [Cheat Sheets][cheatsheet-proactive-c9]
* C10: [Handle all Errors and Exceptions][control10], ref [Cheat Sheets][cheatsheet-proactive-c10]

#### Why use them?

The Proactive Controls are a well established list of security controls, first published in 2014
and revised in 2018, so considering these controls can be seen as best practice.
Following best practice is always encouraged: at the very least an organization should avoid the avoidable exploits.

#### How to apply them

The OWASP Spotlight series provides an overview of how to use this documentation project:
'Project 8 - [Proactive Controls][spotlight08]'.

During development of a web application, consider using each security control
described in the sections of the Proactive Controls that are relevant to the application.

The OWASP Cheat Sheets have been indexed specifically for [each Proactive Control][cheatsheet-proactive],
which can be used as additional information on implementing the control.

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue070101] or [edit on GitHub][edit070101].

[cheatsheet-proactive]: https://cheatsheetseries.owasp.org/IndexProactiveControls
[cheatsheet-proactive-c1]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c1-define-security-requirements
[cheatsheet-proactive-c2]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c2-leverage-security-frameworks-and-libraries
[cheatsheet-proactive-c3]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c3-secure-database-access
[cheatsheet-proactive-c4]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c4-encode-and-escape-data
[cheatsheet-proactive-c5]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c5-validate-all-inputs
[cheatsheet-proactive-c6]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c6-implement-digital-identity
[cheatsheet-proactive-c7]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c7-enforce-access-controls
[cheatsheet-proactive-c8]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c8-protect-data-everywhere
[cheatsheet-proactive-c9]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c9-implement-security-logging-and-monitoring
[cheatsheet-proactive-c10]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c10-handle-all-errors-and-exceptions
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
[edit070101]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/07-implementation/01-documentation/01-proactive-controls.md
[issue070101]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=content&template=request.md&title=Update:%2007-implementation/01-documentation/01-proactive-controls
[proactive10]: https://owasp.org/www-project-proactive-controls/
[proactive10-pdf]: https://github.com/OWASP/www-project-proactive-controls/tree/master/v3
[spotlight08]: https://youtu.be/HRtYDCWOSc0

\newpage
