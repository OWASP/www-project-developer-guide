---

title: Design
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 600
permalink: /release/design/

---

{% include breadcrumb.html %}

## 4. Design

Security Architecture is one of the practices that is described in the [Software Assurance Maturity Model (SAMM)][sammdsa].
Referring to the [Secure Product Design Cheat Sheet][spdcs], the purpose of secure architecture and design is to ensure
that all products meet or exceed the security requirements laid down by the organization,
focusing on the security linked to components and technologies used during the development of the application.

Secure Architecture Design looks at the selection and composition of components that form the foundation of the solution.
Technology Management looks at the security of supporting technologies used during development, deployment and operations,
such as development stacks and tooling, deployment tooling, and operating systems and tooling.

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

Checklists and Cheat Sheets are an important tool during the design process;
they provide an easy reference of knowledge and help avoid repeating design errors and mistakes.

Sections:

4.1 [Threat modeling](01-threat-modeling/toc.md)  
4.1.1 [Threat modeling in practice](01-threat-modeling/01-threat-modeling.md)  
4.1.2 [Pythonic Threat Modeling](01-threat-modeling/02-pytm.md)  
4.1.3 [Threat Dragon](01-threat-modeling/03-threat-dragon.md)  
4.1.4 [Threat Modeling and Cornucopia](01-threat-modeling/04-cornucopia.md)  
4.1.5 [Threat Modeling toolkit](01-threat-modeling/05-toolkit.md)  
4.2 [Web application checklist](02-web-app-checklist/toc.md)  
4.2.1 [Checklist: Define Security Requirements](02-web-app-checklist/01-define-security-requirements.md)  
4.2.2 [Checklist: Leverage Security Frameworks and Libraries](02-web-app-checklist/02-frameworks-libraries.md)  
4.2.3 [Checklist: Secure Database Access](02-web-app-checklist/03-secure-database-access.md)  
4.2.4 [Checklist: Encode and Escape Data](02-web-app-checklist/04-encode-escape-data.md)  
4.2.5 [Checklist: Validate All Inputs](02-web-app-checklist/05-validate-inputs.md)  
4.2.6 [Checklist: Implement Digital Identity](02-web-app-checklist/06-digital-identity.md)  
4.2.7 [Checklist: Enforce Access Controls](02-web-app-checklist/07-access-controls.md)  
4.2.8 [Checklist: Protect Data Everywhere](02-web-app-checklist/08-protect-data.md)  
4.2.9 [Checklist: Implement Security Logging and Monitoring](02-web-app-checklist/09-logging-monitoring.md)  
4.2.10 [Checklist: Handle all Errors and Exceptions](02-web-app-checklist/10-handle-errors-exceptions.md)  
4.3 [Mobile application checklist](03-mas-checklist.md)  

----

[sammdsa]: https://owaspsamm.org/model/design/security-architecture/
[spdcs]: https://cheatsheetseries.owasp.org/cheatsheets/Secure_Product_Design_Cheat_Sheet.html
