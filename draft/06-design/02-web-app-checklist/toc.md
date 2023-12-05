---

title: Checklist and Proactive Controls
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 1400

---

{% include breadcrumb.html %}

## 4.2. Web application checklist

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

4.2.1 [Checklist: Define Security Requirements](01-define-security-requirements.md)  
4.2.2 [Checklist: Leverage Security Frameworks and Libraries](02-frameworks-libraries.md)  
4.2.3 [Checklist: Secure Database Access](03-secure-database-access.md)  
4.2.4 [Checklist: Encode and Escape Data](04-encode-escape-data.md)  
4.2.5 [Checklist: Validate All Inputs](05-validate-inputs.md)  
4.2.6 [Checklist: Implement Digital Identity](06-digital-identity.md)  
4.2.7 [Checklist: Enforce Access Controls](07-access-controls.md)  
4.2.8 [Checklist: Protect Data Everywhere](08-protect-data.md)  
4.2.9 [Checklist: Implement Security Logging and Monitoring](09-logging-monitoring.md)  
4.2.10 [Checklist: Handle all Errors and Exceptions](10-handle-errors-exceptions.md)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0602] or [edit on GitHub][edit0602].

[issue0602]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/02-web-app-checklist/00-toc
[edit0602]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/02-web-app-checklist/toc.md
[asvs]: https://owasp.org/www-project-application-security-verification-standard/
[proactive10]: https://owasp.org/www-project-proactive-controls/
