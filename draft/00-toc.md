---

title: Table of Contents
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 0
permalink: /draft/

---

{% include breadcrumb.html %}

## ![Developer Guide](../assets/images/dg_logo.png){ height=120px }

## OWASP Developer Guide (draft)

_The draft version has the latest contributions to the Developer Guide
and so the content is expected to frequently change._

1 **[Audience](#audience)**

2 **[Background](#background)**

3 **[Introduction](#introduction)**

4 **[Foundations](#foundations)**  
4.1 [Security fundamentals](#security-fundamentals)  
4.2 [Secure development and integration](#secure-development-and-integration)  
4.3 [Principles of security](#principles-of-security)  
4.4 [Principles of cryptography](#principles-of-cryptography)  
4.5 [Top Ten Web Application Security Risks](#top-ten-web-application-security-risks)  

5 **[Security requirements](#security-requirements)**  
5.1 [Introduction](#introduction-to-security-requirements)  
5.2 [Threat modeling](#threat-modeling)  
5.3 [Risk profile](#risk-profile)  

6 **[Secure design](#secure-design)**  
6.1 [Introduction](#introduction-to-secure-design)  
6.2 [Secure coding](#secure-coding)  
6.3 [Cryptographic practices](#cryptographic-practices)  
6.4 [Application spoofing](#application-spoofing)  
6.5 [Content Security Policy (CSP)](#content-security-policy)  
6.6 [Exception and error handling](#exception-and-error-handling)  
6.7 [File management](#file-management)  
6.8 [Memory management](#memory-management)  

7 **[Container security](#container-security)**  
7.1 [Introduction](#introduction-to-container-security)  
7.2 [Image security](#image-security)  
7.3 [Container scanning](#container-scanning)  

8 **[Open-Source software](#open-source-software)**  
8.1 [Introduction](#introduction-to-open-source-software)  
8.2 [Static code analysis](#static-code-analysis)  
8.3 [Third Party Software (TPS) and libraries](#third-party-software-and-libraries)  

9 **[Secure environment](#secure-environment)**  
9.1 [Introduction](#introduction-to-secure-environment)  
9.2 [System hardening](#system-hardening)  
9.3 [File systems and downloads](#file-systems-and-downloads)  

10 **[Security testing and validation](#security-testing-and-validation)**  
10.1 [Introduction](#introduction-to-security-testing-and-validation)  
10.2 [Static Application Security Testing (SAST)](#static-application-security-testing)  
10.3 [Dynamic Application Security Testing (DAST)](#dynamic-application-security-testing)  

10 **[Checklist](#checklist)**  
11.1 [Checklist: Define Security Requirements](#checklist-define-security-requirements)  
11.2 [Checklist: Leverage Security Frameworks and Libraries](#checklist-leverage-security-frameworks-and-libraries)  
11.3 [Checklist: Secure Database Access](#checklist-secure-database-access)  
11.4 [Checklist: Encode and Escape Data](#checklist-encode-and-escape-data)  
11.5 [Checklist: Validate All Inputs](#checklist-validate-all-inputs)  
11.6 [Checklist: Implement Digital Identity](#checklist-implement-digital-identity)  
11.7 [Checklist: Enforce Access Controls](#checklist-enforce-access-controls)  
11.8 [Checklist: Protect Data Everywhere](#checklist-protect-data-everywhere)  
11.9 [Checklist: Implement Security Logging and Monitoring](#checklist-implement-security-logging-and-monitoring)  
11.10 [Checklist: Handle all Errors and Exceptions](#checklist-handle-all-errors-and-exceptions)  

\newpage
