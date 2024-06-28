---

title: Security Fundamentals
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 4010
permalink: /release/foundations/security_fundamentals/

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

CIA is often extended with Authentication, Authorization and Auditing as these are closely linked to CIA concepts.
CIA has a strong dependency on Authentication and Authorization;
the confidentiality and integrity of sensitive data can not be assured without them.
Auditing is added as it can provide the mechanism to ensure proof of any interaction with the system.

#### Authentication

Authentication is about confirming the identity of the entity that wants to interact with a secure system.
For example the entity could be an automated client or a human actor;
in either case authentication is required for a secure application.

#### Authorization

Authorization is about specifying access rights to secure resources (data, services, files, applications, etc).
These rights describe the privileges or access levels related to the resources that are being secured.
Authorization is usually preceded by successful authentication.

#### Auditing

Auditing is about keeping track of implementation-level events, as well as domain-level events taking place in a system.
This helps to provide non-repudiation, which means that changes or actions on the protected system are undeniable.
Auditing can provide not only technical information about the running system,
but also proof that particular actions have been performed.
The typical questions that are answered by auditing are "Who did What, When and potentially How?"

#### Software Assurance Maturity Model

The OWASP Software Assurance Maturity Model [(SAMM)][samm] provides a good context for the scope of software security,
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

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0401] or [edit on GitHub][edit0401].

[issue0401]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2004-foundations/01-security-fundamentals
[edit0401]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/04-foundations/01-security-fundamentals.md
[samm]: https://owaspsamm.org/about/
