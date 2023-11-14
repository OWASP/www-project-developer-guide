---

title: Implementation
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order:

---

{% include breadcrumb.html %}

## 5. Implementation

Implementation is where the application / system begins to take shape; source code is written and tests are created.
The implementation of the application follows a secure development lifecycle, with security built in from the start.

The implementation will fulfil the security requirements according to the design,
and be under a secure method of source code control and storage.
The development team will be referring to documentation advising them of best practices,
they will be using secure libraries wherever possible in addition to checking and tracking external dependencies.

Much of the skill of implementation comes from experience, and taking into account the Do's and Don'ts
of secure development is an important knowledge activity in itself.

Sections:

5.1 [Documentation](#documentation)  
5.1.1 [Top 10 Proactive Controls](#top-proactive-controls)  
5.1.2 [Go Secure Coding Practices](#go-secure-coding-practices)  
5.1.3 [Cheatsheet Series](#cheatsheet-series)  
5.2 [Dependencies](#dependencies)
5.2.1 [Dependency-Check](#dependency-check)  
5.2.2 [Dependency-Track](#dependency-track)  
5.2.3 [CycloneDX](#cyclonedx)  
5.3 [Secure Libraries](#secure-libraries)  
5.3.1 [Enterprise Security API library](#enterprise-security-api-library)  
5.3.2 [CSRFGuard library](#csrfguard-library)  
5.3.3 [OWASP Secure Headers Project](#owasp-secure-headers-project)  
5.4 [Implementation Do's and Don'ts](#implementation-dos-and-donts)  
5.4.1 [Container security](#container-security)  
5.4.2 [Secure coding](#secure-coding)  
5.4.3 [Cryptographic practices](#cryptographic-practices)  
5.4.4 [Application spoofing](#application-spoofing)  
5.4.5 [Content Security Policy (CSP)](#content-security-policy)  
5.4.6 [Exception and error handling](#exception-and-error-handling)  
5.4.7 [File management](#file-management)  
5.4.8 [Memory management](#memory-management)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0700] or a [pull request][pr].

[issue0700]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2007-implementation/00-toc
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls

\newpage
