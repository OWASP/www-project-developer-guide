---

title: Security Fundamentals
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 4010
permalink: /release-pt-br/foundations/security_fundamentals/

---

{% include breadcrumb.html %}

### 2.1 Security fundamentals

The OWASP Software Assurance Maturity Model [(SAMM)][samm] is used throughout this Developer Guide
to provide context for each section. Refer to the section below for a brief introduction to SAMM.

#### Overview

Security is simply about controlling who can interact with your information,
what they can do with it, and when they can interact with it.
These characteristics of security can be described using the CIA triad,
and can be extended using the AAA triad.

#### CIA

CIA stands for Confidentiality, Integrity and Availability,
and it is usually depicted as a triangle representing the strong bonds between its three tenets.
This trio is considered the pillars of application security,
with CIA described as a property of some data or of a process.
Often CIA is extended with AAA: Authorization, Authentication and Auditing.

#### Confidentiality

Confidentiality is the protection of data against unauthorized disclosure;
it is about ensuring that only those with the correct authorization can access the data
and applies to both data at rest and to data in transit.
Confidentiality is also related to the broader concept of data privacy.

#### Integrity

Integrity is about protecting data against unauthorized modification, or assuring data trustworthiness.
The concept contains the notion of data integrity (data has not been changed accidentally or deliberately)
and the notion of source integrity (data came from or was changed by a legitimate source).

#### Availability

Availability is about ensuring the presence of information or resources.
This concept relies not just on the availability of the data itself, for example by using replication of data,
but also on the protection of the services that provide access to the data, for example by using load balancing.

#### AAA

The CIA triad is often extended with Authentication, Authorization and Auditing as these are closely linked to CIA concepts.
CIA has a strong dependency on Authentication and Authorization;
the confidentiality and integrity of sensitive data can not be assured without them.
Auditing is added as it can provide the mechanism to ensure proof of any interaction with the system.

#### Authentication

[Authentication][csauthn] is about confirming the identity of the entity that wants to interact with a secure system.
For example the entity could be an automated client or a human actor;
in either case authentication is required for a secure application.

#### Authorization

[Authorization][csauthz] is about specifying access rights to secure resources (data, services, files, applications, etc).
These rights describe the privileges or access levels related to the resources that are being secured.
Authorization is usually preceded by successful authentication.

#### Auditing

Auditing is about keeping track of implementation-level events, as well as domain-level events taking place in a system.
This helps to provide non-repudiation, which means that changes or actions on the protected system are undeniable.
Auditing can provide not only technical information about the running system,
but also proof that particular actions have been performed.
The typical questions that are answered by auditing are "Who did What, When and potentially How?"

#### Software Assurance Maturity Model

The OWASP Software Assurance Maturity Model ([SAMM][samm]) provides a good context for the scope of software security,
and the foundations of SAMM rely on the security concepts in this section.
The SAMM model describes the five fundamentals of software security, which it calls Business Functions:

* Governance
* Design
* Implementation
* Verification
* Operations

Each of these five fundamentals are further split into three Business Practices:

| Business Function   | Business Practices      |                             |                        |
| ------------------- | ----------------------- | --------------------------- | ---------------------- |
| Governance          | Strategy and Metrics    | Policy and Compliance       | Education and Guidance |
| Design              | Threat Assessment       | Security Requirements       | Security Architecture  |
| Implementation      | Secure Build            | Secure Deployment           | Defect Management      |
| Verification        | Architecture Assessment | Requirements-driven Testing | Security Testing       |
| Operations          | Incident Management     | Environment Management      | Operational Management |

Each Business Practice is further subdivided into two streams,
and the sections in the Developer Guide reference at least one of the Business Functions or Practices in SAMM.

#### Vulnerabilities

NIST defines a [vulnerability][definevuln] as 'Weakness in an information system, system security procedures,
internal controls, or implementation that could be exploited or triggered by a threat source.'

There are many weaknesses or bugs in every large application, but the term vulnerability is generally reserved
for those weaknesses or bugs where there is a risk that a threat actor could exploit it using a threat vector.

Well known security vulnerabilities are :

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

#### References

* OWASP [Cheat Sheet Series][cheatsheets]
* OWASP [Software Assurance Maturity Model][samm] (SAMM)

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0401] or [edit on GitHub][edit0401].

[cheatsheets]: https://cheatsheetseries.owasp.org/
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
[csauthn]: https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet
[csauthz]: https://cheatsheetseries.owasp.org/cheatsheets/Authorization_Cheat_Sheet
[csredirect]: https://cheatsheetseries.owasp.org/cheatsheets/Unvalidated_Redirects_and_Forwards_Cheat_Sheet
[cssql]: https://cheatsheetseries.owasp.org/cheatsheets/SQL_Injection_Prevention_Cheat_Sheet
[csquery]: https://cheatsheetseries.owasp.org/cheatsheets/Query_Parameterization_Cheat_Sheet
[csssrf]:  https://cheatsheetseries.owasp.org/cheatsheets/Server_Side_Request_Forgery_Prevention_Cheat_Sheet
[csxss]: https://cheatsheetseries.owasp.org/cheatsheets/Cross_Site_Scripting_Prevention_Cheat_Sheet
[csxsleaks]: https://cheatsheetseries.owasp.org/cheatsheets/XS_Leaks_Cheat_Sheet
[csxssevade]: https://cheatsheetseries.owasp.org/cheatsheets/XSS_Filter_Evasion_Cheat_Sheet
[csxxe]: https://cheatsheetseries.owasp.org/cheatsheets/XML_External_Entity_Prevention_Cheat_Sheet
[definevuln]: https://csrc.nist.gov/glossary/term/vulnerability
[issue0401]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2004-foundations/01-security-fundamentals
[edit0401]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/04-foundations/01-security-fundamentals.md
[samm]: https://owaspsamm.org/about/
