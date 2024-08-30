---

title: Top 10 Proactive Controls
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 27110
permalink: /release-pt-br/implementation/documentation/proactive_controls/

---

{% include breadcrumb.html %}

### 5.1.1 Top 10 Proactive Controls

The OWASP [Top 10 Proactive Controls][csproactive] describes the most important controls and control categories
that security architects and development teams should consider in web application projects.
The [Proactive Controls project][proactive10] is an OWASP Lab documentation project and
the PDF can be downloaded for [various languages][proactive10-pdf].

#### What are the Top 10 Proactive Controls?

The OWASP Top 10 Proactive Controls 2018 is a list of security techniques that should be considered for web applications.
They are ordered by order of importance, with control number 1 being the most important:

* C1: [Define Security Requirements][control1], ref [Cheat Sheets][csproactive-c1]
* C2: [Leverage Security Frameworks and Libraries][control2], ref [Cheat Sheets][csproactive-c2]
* C3: [Secure Database Access][control3], ref [Cheat Sheets][csproactive-c3]
* C4: [Encode and Escape Data][control4], ref [Cheat Sheets][csproactive-c4]
* C5: [Validate All Inputs][control5], ref [Cheat Sheets][csproactive-c5]
* C6: [Implement Digital Identity][control6], ref [Cheat Sheets][csproactive-c6]
* C7: [Enforce Access Controls][control7], ref [Cheat Sheets][csproactive-c7]
* C8: [Protect Data Everywhere][control8], ref [Cheat Sheets][csproactive-c8]
* C9: [Implement Security Logging and Monitoring][control9], ref [Cheat Sheets][csproactive-c9]
* C10: [Handle all Errors and Exceptions][control10], ref [Cheat Sheets][csproactive-c10]

#### Why use them?

The Proactive Controls are a well established list of security controls, first published in 2014
and revised in 2018, so considering these controls can be seen as best practice.
Following best practice is always encouraged: at the very least an organization should avoid the avoidable exploits.

Putting these proactive controls in place can help remediate common security vulnerabilities, for example:

* [Clickjacking][csclick]
* [Credential Stuffing][cscreds]
* [Cross-site leaks][csxsleaks]
* [Denial of Service][csdos] (DoS) attacks
* DOM based [XSS attacks][csdom] including [DOM Clobbering][csdomclub]
* [IDOR][csidor] (Insecure Direct Object Reference)
* [Injection][csinjection] including [OS Command injection][csosinjection] and [XXE][csxxe]
* LDAP specific [injection attacks][csldap]
* [Prototype pollution][csproto]
* [SSRF][csssrf] attacks
* [SQL injection][cssql] and the use of [Query Parameterization][csquery]
* [Unvalidated redirects and forwards][csredirect]
* [XSS attacks][csxss] and [XSS Filter Evasion][csxssevade]

#### How to apply them

The OWASP Spotlight series provides an overview of how to use this documentation project:
'Project 8 - [Proactive Controls][spotlight08]'.

During development of a web application, consider using each security control
described in the sections of the Proactive Controls that are relevant to the application.

The OWASP Cheat Sheets have been indexed specifically for [each Proactive Control][csproactive],
which can be used as additional information on implementing the control.

#### References

* OWASP [Proactive Controls project][proactive10]
* OWASP Cheat Sheet [Proactive Controls index][csproactive]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue070101] or [edit on GitHub][edit070101].

[csclick]: https://cheatsheetseries.owasp.org/cheatsheets/Clickjacking_Defense_Cheat_Sheet
[cscreds]: https://cheatsheetseries.owasp.org/cheatsheets/Credential_Stuffing_Prevention_Cheat_Sheet
[csdom]: https://cheatsheetseries.owasp.org/cheatsheets/DOM_based_XSS_Prevention_Cheat_Sheet
[csdomclub]: https://cheatsheetseries.owasp.org/cheatsheets/DOM_Clobbering_Prevention_Cheat_Sheet
[csdos]: https://cheatsheetseries.owasp.org/cheatsheets/Denial_of_Service_Cheat_Sheet
[csidor]: https://cheatsheetseries.owasp.org/cheatsheets/Insecure_Direct_Object_Reference_Prevention_Cheat_Sheet
[csinjection]: https://cheatsheetseries.owasp.org/cheatsheets/Injection_Prevention_Cheat_Sheet
[csosinjection]: https://cheatsheetseries.owasp.org/cheatsheets/OS_Command_Injection_Defense_Cheat_Sheet
[csldap]: https://cheatsheetseries.owasp.org/cheatsheets/LDAP_Injection_Prevention_Cheat_Sheet
[csproto]: https://cheatsheetseries.owasp.org/cheatsheets/Prototype_Pollution_Prevention_Cheat_Sheet
[csproactive]: https://cheatsheetseries.owasp.org/IndexProactiveControls
[csproactive-c1]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c1-define-security-requirements
[csproactive-c2]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c2-leverage-security-frameworks-and-libraries
[csproactive-c3]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c3-secure-database-access
[csproactive-c4]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c4-encode-and-escape-data
[csproactive-c5]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c5-validate-all-inputs
[csproactive-c6]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c6-implement-digital-identity
[csproactive-c7]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c7-enforce-access-controls
[csproactive-c8]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c8-protect-data-everywhere
[csproactive-c9]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c9-implement-security-logging-and-monitoring
[csproactive-c10]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c10-handle-all-errors-and-exceptions
[csredirect]: https://cheatsheetseries.owasp.org/cheatsheets/Unvalidated_Redirects_and_Forwards_Cheat_Sheet
[cssql]: https://cheatsheetseries.owasp.org/cheatsheets/SQL_Injection_Prevention_Cheat_Sheet
[csquery]: https://cheatsheetseries.owasp.org/cheatsheets/Query_Parameterization_Cheat_Sheet
[csssrf]:  https://cheatsheetseries.owasp.org/cheatsheets/Server_Side_Request_Forgery_Prevention_Cheat_Sheet
[csxss]: https://cheatsheetseries.owasp.org/cheatsheets/Cross_Site_Scripting_Prevention_Cheat_Sheet
[csxsleaks]: https://cheatsheetseries.owasp.org/cheatsheets/XS_Leaks_Cheat_Sheet
[csxssevade]: https://cheatsheetseries.owasp.org/cheatsheets/XSS_Filter_Evasion_Cheat_Sheet
[csxxe]: https://cheatsheetseries.owasp.org/cheatsheets/XML_External_Entity_Prevention_Cheat_Sheet
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
