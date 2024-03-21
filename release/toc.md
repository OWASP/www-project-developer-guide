---

title: Table of Contents
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 2000
permalink: /release/

---

{% include breadcrumb.html %}

![Developer Guide](../assets/images/dg_logo.png "OWASP Developer Guide"){: height="220px" }

## OWASP Developer Guide

### Release version release-workflow

1 **[Introduction](03-introduction.md)**

2 **[Foundations](04-foundations/toc.md)**  
2.1 [Security fundamentals](04-foundations/01-security-fundamentals.md)  
2.2 [Secure development and integration](04-foundations/02-secure-development.md)  
2.3 [Principles of security](04-foundations/03-security-principles.md)  
2.4 [Principles of cryptography](04-foundations/04-crypto-principles.md)  
2.5 [OWASP Top 10](04-foundations/05-top-ten.md)  
2.6 [Security champions](04-foundations/06-security-champions.md)  

3 **[Requirements](05-requirements/toc.md)**  
3.1 [Requirements in practice](05-requirements/01-requirements.md)  
3.2 [Risk profile](05-requirements/02-risk.md)  
3.3 [Security Knowledge Framework](05-requirements/03-skf.md)  
3.4 [SecurityRAT](05-requirements/04-security-rat.md)  
3.5 [Application Security Verification Standard](05-requirements/05-asvs.md)  
3.6 [Mobile Application Security](05-requirements/06-mas.md)  

4 **[Design](06-design/toc.md)**  
4.1 [Threat modeling](06-design/01-threat-modeling/toc.md)  
4.1.1 [Threat modeling in practice](06-design/01-threat-modeling/01-threat-modeling.md)  
4.1.2 [Pythonic Threat Modeling](06-design/01-threat-modeling/02-pytm.md)  
4.1.3 [Threat Dragon](06-design/01-threat-modeling/03-threat-dragon.md)  
4.1.4 [Threat Modeling and Cornucopia](06-design/01-threat-modeling/04-cornucopia.md)  
4.1.5 [Threat Modeling toolkit](06-design/01-threat-modeling/05-toolkit.md)  
4.2 [Web application checklist](06-design/02-web-app-checklist/toc.md)  
4.2.1 [Checklist: Define Security Requirements](06-design/02-web-app-checklist/01-define-security-requirements.md)  
4.2.2 [Checklist: Leverage Security Frameworks and Libraries](06-design/02-web-app-checklist/02-frameworks-libraries.md)  
4.2.3 [Checklist: Secure Database Access](06-design/02-web-app-checklist/03-secure-database-access.md)  
4.2.4 [Checklist: Encode and Escape Data](06-design/02-web-app-checklist/04-encode-escape-data.md)  
4.2.5 [Checklist: Validate All Inputs](06-design/02-web-app-checklist/05-validate-inputs.md)  
4.2.6 [Checklist: Implement Digital Identity](06-design/02-web-app-checklist/06-digital-identity.md)  
4.2.7 [Checklist: Enforce Access Controls](06-design/02-web-app-checklist/07-access-controls.md)  
4.2.8 [Checklist: Protect Data Everywhere](06-design/02-web-app-checklist/08-protect-data.md)  
4.2.9 [Checklist: Implement Security Logging and Monitoring](06-design/02-web-app-checklist/09-logging-monitoring.md)  
4.2.10 [Checklist: Handle all Errors and Exceptions](06-design/02-web-app-checklist/10-handle-errors-exceptions.md)  
4.3 [Mobile application checklist](06-design/03-mas-checklist.md)  

5 **[Implementation](07-implementation/toc.md)**  
5.1 [Documentation](07-implementation/01-documentation/toc.md)  
5.1.1 [Top 10 Proactive Controls](07-implementation/01-documentation/01-proactive-controls.md)  
5.1.2 [Go Secure Coding Practices](07-implementation/01-documentation/02-go-scp.md)  
5.1.3 [Cheatsheet Series](07-implementation/01-documentation/03-cheatsheets.md)  
5.2 [Dependencies](07-implementation/02-dependencies/toc.md)  
5.2.1 [Dependency-Check](07-implementation/02-dependencies/01-dependency-check.md)  
5.2.2 [Dependency-Track](07-implementation/02-dependencies/02-dependency-track.md)  
5.2.3 [CycloneDX](07-implementation/02-dependencies/03-cyclonedx.md)  
5.3 [Secure Libraries](07-implementation/03-secure-libraries/toc.md)  
5.3.1 [Enterprise Security API library](07-implementation/03-secure-libraries/01-esapi.md)  
5.3.2 [CSRFGuard library](07-implementation/03-secure-libraries/02-csrf-guard.md)  
5.3.3 [OWASP Secure Headers Project](07-implementation/03-secure-libraries/03-secure-headers.md)  
5.4 [Implementation Do's and Don'ts](07-implementation/04-dos-donts/toc.md)  
5.4.1 [Container security](07-implementation/04-dos-donts/01-container-security.md)  
5.4.2 [Secure coding](07-implementation/04-dos-donts/02-secure-coding.md)  
5.4.3 [Cryptographic practices](07-implementation/04-dos-donts/03-cryptographic-practices.md)  
5.4.4 [Application spoofing](07-implementation/04-dos-donts/04-application-spoofing.md)  
5.4.5 [Content Security Policy (CSP)](07-implementation/04-dos-donts/05-content-security-policy.md)  
5.4.6 [Exception and error handling](07-implementation/04-dos-donts/06-exception-error-handling.md)  
5.4.7 [File management](07-implementation/04-dos-donts/07-file-management.md)  
5.4.8 [Memory management](07-implementation/04-dos-donts/08-memory-management.md)  

6 **[Verification](08-verification/toc.md)**  
6.1 [Guides](08-verification/01-guides/toc.md)  
6.1.1 [Web Security Testing Guide](08-verification/01-guides/01-wstg.md)  
6.1.2 [Mobile Application Security](08-verification/01-guides/02-mas.md)  
6.1.3 [Application Security Verification Standard](08-verification/01-guides/03-asvs.md)  
6.2 [Tools](08-verification/02-tools/toc.md)  
6.2.1 [Zed Attack Proxy](08-verification/02-tools/01-zap.md)  
6.2.2 [Amass](08-verification/02-tools/02-amass.md)  
6.2.3 [Offensive Web Testing Framework](08-verification/02-tools/03-owtf.md)  
6.2.4 [Nettacker](08-verification/02-tools/04-nettacker.md)  
6.2.5 [OWASP Secure Headers Project](08-verification/02-tools/05-secure-headers.md)  
6.3 [Frameworks](08-verification/03-frameworks/toc.md)  
6.3.1 [secureCodeBox](08-verification/03-frameworks/01-secure-codebox.md)  
6.4 [Vulnerability management](08-verification/04-vulnerability-management/toc.md)  
6.4.1 [DefectDojo](08-verification/04-vulnerability-management/01-defectdojo.md)  
6.5 [Verification Do's and Don'ts](08-verification/05-dos-donts/toc.md)  
6.5.1 [Secure environment](08-verification/05-dos-donts/01-secure-environment.md)  
6.5.2 [System hardening](08-verification/05-dos-donts/02-system-hardening.md)  
6.5.3 [Open Source software](08-verification/05-dos-donts/03-open-source-software.md)  

7 **[Training and Education](09-training-education/toc.md)**  
7.1 [Vulnerable Applications](09-training-education/01-vulnerable-apps/toc.md)  
7.1.1 [Juice Shop](09-training-education/01-vulnerable-apps/01-juice-shop.md)  
7.1.2 [WebGoat](09-training-education/01-vulnerable-apps/02-webgoat.md)  
7.1.3 [PyGoat](09-training-education/01-vulnerable-apps/03-pygoat.md)  
7.1.4 [Security Shepherd](09-training-education/01-vulnerable-apps/04-security-shepherd.md)  
7.2 [Secure Coding Dojo](09-training-education/02-secure-coding-dojo.md)  
7.3 [Security Knowledge Framework](09-training-education/03-skf.md)  
7.4 [SamuraiWTF](09-training-education/04-samurai-wtf.md)  
7.5 [OWASP Top 10 project](09-training-education/05-top-ten.md)  
7.6 [Mobile Top 10](09-training-education/06-mobile-top-ten.md)  
7.7 [API Top 10](09-training-education/07-api-top-ten.md)  
7.8 [WrongSecrets](09-training-education/08-wrongsecrets.md)  
7.9 [OWASP Snakes and Ladders](09-training-education/09-snakes-ladders.md)  

8 **[Culture building and Process maturing](10-culture-building-process-maturing/toc.md)**  
8.1 [Security Champions Playbook](10-culture-building-process-maturing/01-security-champions-playbook.md)  
8.2 [Software Assurance Maturity Model](10-culture-building-process-maturing/02-samm.md)  
8.3 [Application Security Verification Standard](10-culture-building-process-maturing/03-asvs.md)  
8.4 [Mobile Application Security](10-culture-building-process-maturing/04-mas.md)  

9 **[Operation](11-operation/toc.md)**  
9.1 [ModSecurity Core Rule Set](11-operation/01-modsecurity-crs.md)  
9.2 [Coraza Web Application Firewall](11-operation/02-coraza.md)  
9.3 [ModSecurity Web Application Firewall](11-operation/03-modsecurity.md)  

10 **[Metrics](12-metrics/toc.md)**  

11 **[Security gap analysis](13-security-gap-analysis/01-guides/toc.md)**  
11.1 [Guides](13-security-gap-analysis/01-guides/toc.md)  
11.1.1 [Software Assurance Maturity Model](13-security-gap-analysis/01-guides/01-samm.md)  
11.1.2 [Application Security Verification Standard](13-security-gap-analysis/01-guides/02-asvs.md)  
11.1.3 [Mobile Application Security](13-security-gap-analysis/01-guides/03-mas.md)  
11.2 [Bug Logging Tool](13-security-gap-analysis/02-blt.md)  
