---

title: Checklist and Proactive Controls
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order:

---

{% include breadcrumb.html %}

## 12. Checklist

Checklists are a valuable resource for development teams.
They provide structure for establishing good practices and processes
and are also useful during code reviews and design activities.

The checklists that follow are general lists that are categorised to follow the controls listed in the
[OWASP Top 10 Proactive Controls][proactive10] project.
These checklists provide suggestions that certainly should be tailored to
an individual project's requirements and environment; they are not meant to be followed in their entirety.

Probably the best advice on checklists is given by the [Application Security Verification Standard (ASVS)][asvs].
The ASVS can be used to provide a framework for an initial checklist, according to the security verification level,
and this initial ASVS checklist can then be expanded using the following checklist sections.

Sections:

12.1 [Checklist: Define Security Requirements](#checklist-define-security-requirements)  
12.2 [Checklist: Leverage Security Frameworks and Libraries](#checklist-leverage-security-frameworks-and-libraries)  
12.3 [Checklist: Secure Database Access](#checklist-secure-database-access)  
12.4 [Checklist: Encode and Escape Data](#checklist-encode-and-escape-data)  
12.5 [Checklist: Validate All Inputs](#checklist-validate-all-inputs)  
12.6 [Checklist: Implement Digital Identity](#checklist-implement-digital-identity)  
12.7 [Checklist: Enforce Access Controls](#checklist-enforce-access-controls)  
12.8 [Checklist: Protect Data Everywhere](#checklist-protect-data-everywhere)  
12.9 [Checklist: Implement Security Logging and Monitoring](#checklist-implement-security-logging-and-monitoring)  
12.10 [Checklist: Handle all Errors and Exceptions](#checklist-handle-all-errors-and-exceptions)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue1400] or a [pull request][pr].

[issue1400]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2014-checklist/00-toc
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls
[asvs]: https://owasp.org/www-project-application-security-verification-standard/
[proactive10]: https://owasp.org/www-project-proactive-controls/

\newpage
