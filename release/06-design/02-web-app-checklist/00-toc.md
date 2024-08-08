---

title: Web Application Checklist
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order:

---

{% include breadcrumb.html %}

![Developer guide logo](../../../assets/images/dg_logo_bbd.png "OWASP Developer Guide"){height=180px}

### 4.2 Web application checklist

Checklists are a valuable resource for development teams.
They provide structure for establishing good practices and processes
and are also useful during code reviews and design activities.

The checklists that follow are general lists that are categorised to follow the controls listed in the
[OWASP Top 10 Proactive Controls][proactive10] project.
These checklists provide suggestions that certainly should be tailored to
an individual project's requirements and environment; they are not meant to be followed in their entirety.

Probably the best starting point for a checklist is given by the [Application Security Verification Standard (ASVS)][asvs].
The ASVS can be used to provide a framework for an initial checklist, according to the security verification level,
and this initial ASVS checklist can then be expanded using the following checklist sections.

Sections:

4.2.1 [Checklist: Define Security Requirements](#checklist-define-security-requirements)  
4.2.2 [Checklist: Leverage Security Frameworks and Libraries](#checklist-leverage-security-frameworks-and-libraries)  
4.2.3 [Checklist: Secure Database Access](#checklist-secure-database-access)  
4.2.4 [Checklist: Encode and Escape Data](#checklist-encode-and-escape-data)  
4.2.5 [Checklist: Validate All Inputs](#checklist-validate-all-inputs)  
4.2.6 [Checklist: Implement Digital Identity](#checklist-implement-digital-identity)  
4.2.7 [Checklist: Enforce Access Controls](#checklist-enforce-access-controls)  
4.2.8 [Checklist: Protect Data Everywhere](#checklist-protect-data-everywhere)  
4.2.9 [Checklist: Implement Security Logging and Monitoring](#checklist-implement-security-logging-and-monitoring)  
4.2.10 [Checklist: Handle all Errors and Exceptions](#checklist-handle-all-errors-and-exceptions)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing then [submit an issue][issue0602].

[asvs]: https://owasp.org/www-project-application-security-verification-standard/
[issue0602]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/02-web-app-checklist/00-toc
[proactive10]: https://owasp.org/www-project-proactive-controls/
