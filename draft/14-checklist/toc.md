---

title: Proactive Controls Checklist overview
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 1400

---

{% include breadcrumb.html %}

## 14. Checklist

Checklists are a valuable resource for development teams.
They provide structure for establishing good practices and processes
and are also useful during code reviews and design activities.

The checklists that follow are general lists that are categorised to follow the controls listed in the
'[OWASP Top 10 Proactive Controls][proactive10]' project.
These checklists provide suggestions that certainly should be tailored to
an individual project's requirements and environment; they are not meant to be followed in their entirety.

Probably the best advice on checklists is given by the [Application Security Verification Standard (ASVS)][asvs].
The ASVS can be used to provide a framework for an initial checklist, according to the security verification level,
and the initial ASVS checklist can then be expanded using the following checklist sections.

Sections:

14.1 [Checklist: Define Security Requirements](01-define-security-requirements.md)  
14.2 [Checklist: Leverage Security Frameworks and Libraries](02-frameworks-libraries.md)  
14.3 [Checklist: Secure Database Access](03-secure-database-access.md)  
14.4 [Checklist: Encode and Escape Data](04-encode-escape-data.md)  
14.5 [Checklist: Validate All Inputs](05-validate-inputs.md)  
14.6 [Checklist: Implement Digital Identity](06-digital-identity.md)  
14.7 [Checklist: Enforce Access Controls](07-access-controls.md)  
14.8 [Checklist: Protect Data Everywhere](08-protect-data.md)  
14.9 [Checklist: Implement Security Logging and Monitoring](09-logging-monitoring.md)  
14.10 [Checklist: Handle all Errors and Exceptions](10-handle-errors-exceptions.md)  

[asvs]: https://owasp.org/www-project-application-security-verification-standard/
[proactive10]: https://owasp.org/www-project-proactive-controls/
