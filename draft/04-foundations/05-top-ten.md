---

title: OWASP Top Ten
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 405

---

{% include breadcrumb.html %}

### 4.5 OWASP Top Ten

The OWASP Top Ten is a very well known list of web application security risks,
and is included by the OWASP Software Assurance Maturity Model [(SAMM)][samm]
in the Education & Guidance practice within the Governance business function.

### Overview

The OWASP [Top 10 Web Application Security Risks][top10] project is probably the most well known security concept
within the security community, achieving wide spread acceptance and fame soon after its release in 2003.
Often referred to as just the 'OWASP Top Ten', it is a list that identifies the most important threats
to web applications and seeks to rank them in importance / severity.

The list has changed over time, with some threat types becoming more of a problem to web applications
and other threats have becoming less of a risk as technologies change.
The latest version was issued in 2021 and is summarised below.

Note that there are various 'OWASP Top Ten' projects, for example the 'OWASP Top 10 for Large Language Model Applications',
so to avoid confusion the context should be noted when referring to these lists.

#### A01:2021 Broken Access Control

Access control involves the use of protection mechanisms that can be categorized as:

* Authentication (proving the identity of an actor)
* Authorization (ensuring that a given actor can access a resource)
* Accountability (tracking of activities that were performed)

Broken Access Control is where the product does not restrict, or incorrectly restricts, access to a resource
from an unauthorized or malicious actor.
When a security control fails or is not applied then attackers can compromise the security of the product
by gaining privileges, reading sensitive information, executing commands, evading detection, etc.

Broken Access Control can take many forms, such as path traversal or elevation of privilege, 
so refer to both the [Common Weakness Enumeration CWE-284][cwe284] and [OWASP Top 10 A01:2021][a01]
for examples and follow the various [OWASP Cheat Sheets][a01cs] related to access controls.

#### A02:2021 Cryptographic Failures

Referring to [OWASP Top 10 A02:2021][a02], sensitive data should be protected when at rest and in transit.
Cryptographic failures occur when the cryptographic security control is either broken or not applied,
and the data is exposed to unauthorized actors (malicious or not).

It is important to protect data both at rest, when it is stored in an area  of memory,
and also when it is in transit such as being transmitted across a communication channel or being transformed.
A good example of protecting data transformation is given by [A02 Cryptographic Failures][a02]
where sensitive data is properly encrypted in a database, but the export function automatically
decrypts the data leading to sensitive data exposure.

Crypto failures can take many forms and may be subtle - a security control that looks secure may be easily broken.
Follow the crypto [OWASP Cheat Sheets][a02cs] to get the basic crypto controls in place
and consider arranging for a crypto audit.

#### A03:2021 Injection

A lack of input validation and sanitization can lead to injection exploits,
and this risk has been a constant feature of the OWASP Top Ten since the beginning.
These vulnerabilities occur when hostile data is directly used within the application
and can result in malicious data being used to subvert the application; see [A03 Injection][a03] for further explanations.

The security control is straight forward: all input from untrusted sources should be sanitized and validated.
See the [Injection Cheat Sheets][a03cs] for the varius types of input and their controls.

#### A04:2021 Insecure Design

#### A05:2021 Security Misconfiguration

#### A06:2021 Vulnerable and Outdated Components

#### A07:2021 Identification and Authentication Failures

#### A08:2021 Software and Data Integrity Failures

#### A09:2021 Security Logging and Monitoring Failures

#### A10:2021 Server-Side Request Forgery

### OWASP top tens

There are various 'Top 10' projects created by OWASP that, depending on the context,
may also be referred to as 'OWASP Top 10'.
Here is a list of the stable 'OWASP Top 10' projects:

* [API Security Top 10][api10]
* [Data Security Top 10][data10]
* [Low-Code/No-Code Top 10][lcnc10]
* [Mobile Top 10][mobile10]
* [Top 10 CI/CD Security Risks][cicd10]
* [Top 10 for Large Language Model Applications][llm10]
* [Top 10 Privacy Risks][privacy10]
* [Top 10 Proactive Controls][proactive10]
* [Top 10 Web Application Security Risks][top10]

There are other OWASP Top 10s that are still being worked on as 'incubator' projects so this list is subject to change.

### OWASP Top 10 versions

The OWASP Top 10 Web Application Security Risks document was originally published in 2003,
making it one of our longest lived OWASP projects.
Listed below are the versions up to the latest in 2021, which was released to mark 20 years of OWASP.

* Original [2003](https://github.com/OWASP/Top10/blob/master/archives/OWASPWebApplicationSecurityTopTen-Version1.pdf)
* [2004](https://github.com/OWASP/Top10/blob/master/archives/OWASP_Top_Ten_2004.pdf)
* [2007](https://owasp.org/www-pdf-archive//OWASP_Top_10_2007.pdf)
* [2010](https://github.com/OWASP/OWASP-Top-10/tree/master/2010)
* [2013](https://github.com/OWASP/Top10/tree/master/2013)
* [2017](https://github.com/OWASP/Top10/tree/master/2017)
* Latest [2021](https://github.com/OWASP/Top10/tree/master/2021)

----

The OWASP Developer Guide is a community effort; if you see something that needs changing
then [submit an issue][issue0405] or a [pull request][pr] .

[a01]: https://owasp.org/Top10/A01_2021-Broken_Access_Control/
[a01cs]: https://cheatsheetseries.owasp.org/IndexTopTen.html#a012021-broken-access-control
[a02]: https://owasp.org/Top10/A02_2021-Cryptographic_Failures/
[a02cs]: https://cheatsheetseries.owasp.org/IndexTopTen.html#a022021-cryptographic-failures
[a03]: https://owasp.org/Top10/A03_2021-Injection/
[a03cs]: https://cheatsheetseries.owasp.org/IndexTopTen.html#a032021-injection
[api10]: https://owasp.org/www-project-api-security/
[cicd10]: https://owasp.org/www-project-top-10-ci-cd-security-risks/
[cwe284]: https://cwe.mitre.org/data/definitions/284.html
[data10]: https://owasp.org/www-project-data-security-top-10/
[issue0405]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2004-foundations/05-top-ten
[lcnc10]: https://owasp.org/www-project-top-10-low-code-no-code-security-risks/
[mobile10]: https://owasp.org/www-project-mobile-top-10/
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls
[privacy10]: https://owasp.org/www-project-top-10-privacy-risks/
[proactive10]: https://owasp.org/www-project-proactive-controls/
[samm]: https://owaspsamm.org/about/
[top10]: https://owasp.org/www-project-top-ten/
[llm10]: https://owasp.org/www-project-top-10-for-large-language-model-applications/

\newpage
