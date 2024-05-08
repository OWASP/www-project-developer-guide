---

title: Requirements
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 5000
permalink: /release/requirements/

---

{% include breadcrumb.html %}

## 3. Requirements

Referring to the OWASP [Top Ten Proactive Controls][control1], security requirements are statements of
security functionality that ensure the different security properties of a software application are being satisfied.
Security requirements are derived from industry standards, applicable laws, and a history of past vulnerabilities.
Security requirements define new features or additions to existing features to solve a specific security problem
or eliminate potential vulnerabilities.

Security requirements also provide a foundation of vetted security functionality for an application.
Instead of creating a custom approach to security for every application,
standard security requirements allow developers to reuse the definition of security controls and best practices;
those same vetted security requirements provide solutions for security issues that have occurred in the past.

The importance of understanding key security requirements is described in the [Security Requirements][sammdsr]
practice that is part of the [Design][sammd] business function section within the OWASP [SAMM model][samm].
Ideally structured software security requirements are available within with a security a requirements framework,
and these are utilized by both developer teams and product teams.
In addition suppliers to the organization must meet security requirements;
build security into supplier agreements in order to ensure compliance with organizational security requirements.

In summary, security requirements exist to prevent the repeat of past security failures.

Sections:

3.1 [Requirements in practice](01-requirements.md)  
3.2 [Risk profile](02-risk.md)  
3.3 [Security Knowledge Framework](03-skf.md)  
3.4 [SecurityRAT](04-security-rat.md)  
3.5 [Application Security Verification Standard](05-asvs.md)  
3.6 [Mobile Application Security](06-mas.md)  

----

[control1]: https://owasp.org/www-project-proactive-controls/v3/en/c1-security-requirements
[samm]: https://owaspsamm.org/about/
[sammd]: https://owaspsamm.org/model/design/
[sammdsr]: https://owaspsamm.org/model/design/security-requirements/
