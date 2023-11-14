---

title: Design
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order:

---

{% include breadcrumb.html %}

## 4. Design

Referring to the [Secure Product Design Cheat Sheet][spdcs], the purpose of secure product design is to ensure
that all products meet or exceed the security requirements laid down by the organization.

A secure design will help establish secure defaults, minimise the attack surface area
and fail securely to well-defined and understood defaults.
It will also consider and follow various principles, such as:

* Least Privilege and Separation of Duties
* Defense-in-Depth
* Zero Trust
* Security in the Open

A Secure Development Lifecycle (SDLC) helps to ensure that all security decisions made about the product being developed
are explicit choices and result in the correct level of security for the product design.
Various secure development lifecycles can be used and they generally include threat modeling in the design process.

Checklists are an important tool during the design process;
they provide an easy reference of knowledge and help avoid repeating design errors and mistakes.

Sections:

4.1 [Threat modeling](#threat-modeling)  
4.1.1 [Threat modeling in practice](#threat-modeling-in-practice)  
4.1.2 [Pythonic Threat Modeling](#pythonic-threat-modeling)  
4.1.3 [Threat Dragon](#threat-dragon)  
4.1.4 [Threat Modeling and Cornucopia](#cornucopia)  
4.1.5 [Threat Modeling toolkit](#threat-modeling-toolkit)  
4.2 [Web application checklist](#web-application-checklist)  
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
4.3 [Mobile application checklist](#mobile-application-checklist)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0600] or a [pull request][pr].

[issue0600]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/00-toc
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls
[spdcs]: https://cheatsheetseries.owasp.org/cheatsheets/Secure_Product_Design_Cheat_Sheet.html

\newpage
