---

title: Diseño
layout: col-document
tags: Guía del Desarrollador OWASP
contributors:
document: Guía del Desarrollador OWASP
order:

---

{% include breadcrumb.html %}

![WIP logo](../../../assets/images/dg_wip.png "Trabajo en curso"){height=180px}

## 4. Diseño

No hay traducción de esta página, consulte [versión original en inglés][release0600].

Sections:

4.1 [Threat modeling](#threat-modeling)  
4.1.1 [Threat modeling in practice](#threat-modeling-in-practice)  
4.1.2 [pytm](#pytm)  
4.1.3 [Threat Dragon](#threat-dragon)  
4.1.4 [Cornucopia](#cornucopia)  
4.1.5 [LINDDUN GO](#linddun-go)  
4.1.6 [Threat Modeling toolkit](#threat-modeling-toolkit)  
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

[release0600]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/06-design/toc.md

\newpage
