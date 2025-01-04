---

title: Table of Contents
layout: col-document
tags: Guia do Desenvolvedor do OWASP
contributors:
document: Guia do Desenvolvedor do OWASP
order:
permalink:

---

{% include breadcrumb.html %}

## Table of contents

1 **[Introdução](#introduction)**  

2 **[Fundamentos](#foundations)**  
2.1 [Fundamentos de segurança](#security-fundamentals)  
2.2 [Desenvolvimento e integração seguros](#secure-development-and-integration)  
2.3 [Princípios de segurança](#principles-of-security)  
2.4 [Princípios de criptografia](#principles-of-cryptography)  
2.5 [OWASP Top 10](#owasp-top-ten)  

3 **[Requisitos](#requirements)**  
3.1 [Requisitos em prática](#requirements-in-practice)  
3.2 [Perfil de risco](#risk-profile)  
3.3 [OpenCRE](#opencre)  
3.4 [SecurityRAT](#security-rat)  
3.5 [ASVS (Padrão de Verificação de Segurança de Aplicações)](#application-security-verification-standard)  
3.6 [MAS (Segurança de Aplicativos Móveis](#mobile-application-security)  
3.7 [SKF (Framework de Conhecimento de Segurança)](#security-knowledge-framework)  

4 **[Design](#design)**  
4.1 [Modelagem de ameaças](#threat-modeling)  
4.1.1 [Modelagem de ameaças em prática](#threat-modeling-in-practice)  
4.1.2 [pytm](#pytm)  
4.1.3 [Threat Dragon](#threat-dragon)  
4.1.4 [Cornucopia](#cornucopia)  
4.1.5 [LINDDUN GO](#linddun-go)  
4.1.6 [Toolkit para Modelagem de Ameaças](#threat-modeling-toolkit)  
4.2 [Lista de verificação para aplicação web](#web-application-checklist)  
4.2.1 [Defina Requisitos de Segurança](#checklist-define-security-requirements)  
4.2.2 [Leverage Security Frameworks and Libraries](#checklist-leverage-security-frameworks-and-libraries)  
4.2.3 [Secure Database Access](#checklist-secure-database-access)  
4.2.4 [Codifique e Escape Dados](#checklist-encode-and-escape-data)  
4.2.5 [Valide todas as entradas](#checklist-validate-all-inputs)  
4.2.6 [Implement Digital Identity](#checklist-implement-digital-identity)  
4.2.7 [Enforce Access Controls](#checklist-enforce-access-controls)  
4.2.8 [Protect Data Everywhere](#checklist-protect-data-everywhere)  
4.2.9 [Implemente Registro e Monitoramento de Segurança](#checklist-implement-security-logging-and-monitoring)  
4.2.10 [Handle all Errors and Exceptions](#checklist-handle-all-errors-and-exceptions)  
4.3 [MAS Lista de verificação](#mobile-application-checklist)  

5 **[Implementação](#implementation)**  
5.1 [Documentação](#documentation)  
5.1.1 [Top 10 Controles Proativos](#top-proactive-controls)  
5.1.2 [GoSCP (Práticas de Codificação Segura em Go)](#go-secure-coding-practices)  
5.1.3 [Série de Cheatsheet](#cheatsheet-series)  
5.2 [Dependências](#dependencies)
5.2.1 [Dependency-Check](#dependency-check)  
5.2.2 [Dependency-Track](#dependency-track)  
5.2.3 [CycloneDX](#cyclonedx)  
5.3 [Bibliotecas Seguras](#secure-libraries)  
5.3.1 [ESAPI (Biblioteca de API de Segurança Corporative)](#enterprise-security-api-library)  
5.3.2 [CSRFGuard](#csrfguard-library)  
5.3.3 [OSHP (Projeto de Cabeçalhos Seguros OWASP)](#owasp-secure-headers-project)  

6 **[Verification](#verification)**  
6.1 [Guides](#verification-guides)  
6.1.1 [Web Security Testing Guide](#web-security-testing-guide)  
6.1.2 [MAS Testing Guide](#mas-testing-guide)  
6.1.3 [Application Security Verification Standard](#application-security-verification-standard)  
6.2 [Tools](#verification-tools)  
6.2.1 [DAST tools](#dast-tools)  
6.2.2 [Amass](#amass)  
6.2.3 [Offensive Web Testing Framework](#offensive-web-testing-framework)  
6.2.4 [Nettacker](#nettacker)  
6.2.5 [OWASP Secure Headers Project](#secure-headers-project)  
6.3 [Frameworks](#verification-frameworks)  
6.3.1 [secureCodeBox](#securecodebox)  
6.4 [Vulnerability management](#verification-vulnerability-management)  
6.4.1 [DefectDojo](#defectdojo)  

7 **[Training and Education](#training-and-education)**  
7.1 [Vulnerable Applications](#vulnerable-applications)  
7.1.1 [Juice Shop](#juice-shop)  
7.1.2 [WebGoat](#webgoat)  
7.1.3 [PyGoat](#pygoat)  
7.1.4 [Security Shepherd](#security-shepherd)  
7.2 [Secure Coding Dojo](#secure-coding-dojo)  
7.3 [SKF training](#security-knowledge-framework-training)  
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

9 **[Operations](#operations)**  
9.1 [DevSecOps Guideline](#devsecops-guideline)  
9.2 [Coraza Web Application Firewall](#coraza-web-application-firewall)  
9.3 [ModSecurity Web Application Firewall](#modsecurity-web-application-firewall)  
9.4 [OWASP CRS](#owasp-crs)  

10 **[Metrics](#metrics)**  

11 **[Security gap analysis](#security-gap-analysis)**  
11.1 [Guides](#security-gap-analysis-guides)  
11.1.1 [Software Assurance Maturity Model](#software-assurance-maturity-model)  
11.1.2 [Application Security Verification Standard](#application-security-verification-standard)  
11.1.3 [Mobile Application Security](#mobile-application-security)  
11.2 [Bug Logging Tool](#bug-logging-tool)  

12 **[Appendices](#appendices)**  
12.1 [Implementation Do's and Don'ts](#implementation-dos-and-donts)  
12.1.1 [Container security](#container-security)  
12.1.2 [Secure coding](#secure-coding)  
12.1.3 [Cryptographic practices](#cryptographic-practices)  
12.1.4 [Application spoofing](#application-spoofing)  
12.1.5 [Content Security Policy (CSP)](#content-security-policy)  
12.1.6 [Exception and error handling](#exception-and-error-handling)  
12.1.7 [File management](#file-management)  
12.1.8 [Memory management](#memory-management)  
12.2 [Verification Do's and Don'ts](#verification-dos-and-donts)  
12.2.1 [Secure environment](#secure-environment)  
12.2.2 [System hardening](#system-hardening)  
12.2.3 [Open Source software](#open-source-software)  
