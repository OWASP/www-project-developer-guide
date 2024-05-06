---

title: Table of Contents
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order:
permalink:

---

{% include breadcrumb.html %}

## Table of contents

1 **[Introduction](#introduction)**  

2 **[Foundations](#foundations)**  
2.1 [Security fundamentals](#security-fundamentals)  
2.2 [Secure development and integration](#secure-development-and-integration)  
2.3 [Principles of security](#principles-of-security)  
2.4 [Principles of cryptography](#principles-of-cryptography)  
2.5 [OWASP Top 10](#owasp-top-ten)  

3 **[Requirements](#requirements)**  
3.1 [Requirements in practice](#requirements-in-practice)  
3.2 [Risk profile](#risk-profile)  
3.3 [Security Knowledge Framework](#security-knowledge-framework)  
3.4 [SecurityRAT](#security-rat)  
3.5 [Application Security Verification Standard](#application-security-verification-standard)  
3.6 [Mobile Application Security](#mobile-application-security)  

4 **[Design](#design)**  
4.1 [Threat modeling](#threat-modeling)  
4.1.1 [Threat modeling in practice](#threat-modeling-in-practice)  
4.1.2 [Pythonic Threat Modeling](#pythonic-threat-modeling)  
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

5 **[Implementation](#implementation)**  
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

6 **[Verification](#verification)**  
6.1 [Guides](#verification-guides)  
6.1.1 [Web Security Testing Guide](#web-security-testing Guide)  
6.1.2 [Mobile Application Security](#mobile-application-security)  
6.1.3 [Application Security Verification Standard](#application-security-verification-standard)  
6.2 [Tools](#verification-tools)  
6.2.1 [Zed Attack Proxy](#zed-attack-proxy)  
6.2.2 [Amass](#amass)  
6.2.3 [Offensive Web Testing Framework](#offensive-web-testing-framework)  
6.2.4 [Nettacker](#nettacker)  
6.2.5 [OWASP Secure Headers Project](#secure-headers-project)  
6.3 [Frameworks](#verification-frameworks)  
6.3.1 [secureCodeBox](#securecodebox)  
6.4 [Vulnerability management](#verification-vulnerability-management)  
6.4.1 [DefectDojo](#defectdojo)  
6.5 [Verification Do's and Don'ts](#verification-dos-and-donts)  
6.5.1 [Secure environment](#secure-environment)  
6.5.2 [System hardening](#system-hardening)  
6.5.3 [Open Source software](#open-source-software)  

7 **[Training and Education](#training-and-education)**  
7.1 [Vulnerable Applications](#vulnerable-applications)  
7.1.1 [Juice Shop](#juice-shop)  
7.1.2 [WebGoat](#webgoat)  
7.1.3 [PyGoat](#pygoat)  
7.1.4 [Security Shepherd](#security-shepherd)  
7.2 [Secure Coding Dojo](#secure-coding-dojo)  
7.3 [Security Knowledge Framework](#security-knowledge-framework-training)  
7.4 [SamuraiWTF](#samuraiwtf)  
7.5 [OWASP Top 10 project](#owasp-top-ten-project)  
7.6 [Mobile Top 10](#mobile-top-ten)  
7.7 [API Top 10](#api-top-ten)  
7.8 [WrongSecrets](#wrongsecrets)  
7.9 [OWASP Snakes and Ladders](#owasp-snakes-and-ladders)  

8 **[Culture building and Process maturing](#culture-building-and-process-maturing)**  
8.1 [Security Culture](#security-culture)  
8.2 [Security Champions](#security-champions)  
8.2.1 [Security champions program](#security-champions-program)  
8.2.2 [Security Champions Guide](#security-champions-guide)  
8.2.3 [Security Champions Playbook](#security-champions-playbook)  
8.3 [Software Assurance Maturity Model](#software-assurance-maturity-model)  
8.4 [Application Security Verification Standard](#application-security-verification-standard)  
8.5 [Mobile Application Security](#mobile-application-security)  

9 **[Operation](#operation)**  
9.1 [ModSecurity Core Rule Set](#modSecurity-core-rule-set)  
9.2 [Coraza Web Application Firewall](#coraza-web-application-firewall)  
9.3 [ModSecurity Web Application Firewall](#modsecurity-web-application-firewall)  
9.4 [ModSecurity Core Rule Set](#modSecurity-core-rule-set)  

10 **[Metrics](#metrics)**  

11 **[Security gap analysis](#security-gap-analysis)**  
11.1 [Guides](#security-gap-analysis-guides)  
11.1.1 [Software Assurance Maturity Model](#software-assurance-maturity-model)  
11.1.2 [Application Security Verification Standard](#application-security-verification-standard)  
11.1.3 [Mobile Application Security](#mobile-application-security)  
11.2 [Bug Logging Tool](#bug-logging-tool)  

\newpage
