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
6.1 [Guias](#verification-guides)  
6.1.1 [WSTG (Guia de Testes de Segurança para Aplicações Web)](#web-security-testing-guide)  
6.1.2 [MASTG (Guia de Tests MAS)](#mas-testing-guide)  
6.1.3 [ASVS (Padrão de Verificação de Segurança de Aplicações)](#application-security-verification-standard)  
6.2 [Ferramentas verificação](#verification-tools)  
6.2.1 [Ferramentas DAST](#dast-tools)  
6.2.2 [Amass](#amass)  
6.2.3 [OWTF (Framework de Teste Ofensivo de Web)](#offensive-web-testing-framework)  
6.2.4 [Nettacker](#nettacker)  
6.2.5 [OSHP (Projeto de Cabeçalhos Seguros OWASP)](#secure-headers-project)  
6.3 [Verificacao frameworks](#verification-frameworks)  
6.3.1 [secureCodeBox](#securecodebox)  
6.4 [Gerenciamento de vulnerabilidades](#verification-vulnerability-management)  
6.4.1 [DefectDojo](#defectdojo)  

7 **[Treinamento e Educação](#training-and-education)**  
7.1 [Aplicações Vulneráveis](#vulnerable-applications)  
7.1.1 [Juice Shop](#juice-shop)  
7.1.2 [WebGoat](#webgoat)  
7.1.3 [PyGoat](#pygoat)  
7.1.4 [Security Shepherd](#security-shepherd)  
7.2 [Secure Coding Dojo](#secure-coding-dojo)  
7.3 [SKF training](#security-knowledge-framework-training)  
7.4 [SamuraiWTF](#samuraiwtf)  
7.5 [Projeto OWASP Top 10](#owasp-top-ten-project)  
7.6 [Mobile Top 10](#mobile-top-ten)  
7.7 [API Top 10](#api-top-ten)  
7.8 [WrongSecrets](#wrongsecrets)  
7.9 [OWASP Snakes and Ladders](#owasp-snakes-and-ladders)  

8 **[Construção de cultura e Amadurecimento de processos](#culture-building-and-process-maturing)**  
8.1 [Cultura de Segurança](#security-culture)  
8.2 [Campeões de Segurança](#security-champions)  
8.2.1 [Programa de Campeões de Segurança](#security-champions-program)  
8.2.2 [Guia de Campeões de Segurança](#security-champions-guide)  
8.2.3 [Security Champions Playbook](#security-champions-playbook)  
8.3 [SAMM (Modelo de Maturidade de Software Assurance)](#software-assurance-maturity-model)  
8.4 [ASVS (Padrão de Verificação de Segurança de Aplicações)](#application-security-verification-standard)  
8.5 [MAS (Segurança de Aplicativos Móveis)](#mobile-application-security)  

9 **[Operações](#operations)**  
9.1 [Diretriz de DevSecOps](#devsecops-guideline)  
9.2 [Coraza Web Application Firewall](#coraza-web-application-firewall)  
9.3 [ModSecurity Web Application Firewall](#modsecurity-web-application-firewall)  
9.4 [OWASP CRS](#owasp-crs)  

10 **[Métricas](#metricas)**  

11 **[Análise de lacunas de segurança](#security-gap-analysis)**  
11.1 [Guias](#security-gap-analysis-guides)  
11.1.1 [SAMM (Modelo de Maturidade de Software Assurance)](#software-assurance-maturity-model)  
11.1.2 [ASVS (adrão de Verificação de Segurança de Aplicações)](#application-security-verification-standard)  
11.1.3 [MAS (Segurança de Aplicativos Móveis)](#mobile-application-security)  
11.2 [BLT (Ferramenta de registro de bugs)](#bug-logging-tool)  

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
