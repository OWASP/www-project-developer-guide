---

title: Requirements
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 500

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

So you can look at it this way: requirements exist to prevent the repeat of past security failures.

Sections:

3.1 [Requirements in practice](01-requirements.md)  
3.2 [Risk profile](02-risk.md)  
3.3 [Security Knowledge Framework](03-skf.md)  
3.4 [Security RAT](04-security-rat.md)  
3.5 [Application Security Verification Standard](05-asvs.md)  
3.6 [Mobile Application Security](06-mas.md)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0500] or [edit on GitHub][edit0500].

[control1]: https://owasp.org/www-project-proactive-controls/v3/en/c1-security-requirements
[issue0500]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2005-requirements/00-toc
[edit0500]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/05-requirements/toc.md
