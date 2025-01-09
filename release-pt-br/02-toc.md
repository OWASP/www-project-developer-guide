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

1 **[Introdução](#introdução)**  

2 **[Fundamentos](#fundamentos)**  
2.1 [Fundamentos de segurança](#fundamentos-de-segurança)  
2.2 [Desenvolvimento e integração seguros](#desenvolvimento-e-integração-seguros)  
2.3 [Princípios de segurança](#princípios-de-segurança)  
2.4 [Princípios de criptografia](#princípios-de-criptografia)  
2.5 [OWASP Top 10](#owasp-top-ten)  

3 **[Requisitos](#requisitos)**  
3.1 [Requisitos na prática](#requisitos-na-prática)  
3.2 [Perfil de risco](#perfil-de-risco)  
3.3 [OpenCRE](#opencre)  
3.4 [SecurityRAT](#securityrat)  
3.5 [ASVS Requisitos](#asvs-requisitos)  
3.6 [MAS Requisitos](#mas-requisitos)  
3.7 [SKF Requisitos](#skf-requisitos)  

4 **[Design](#design)**  
4.1 [Modelagem de ameaças](#modelagem-de-ameaças)  
4.1.1 [Modelagem de ameaças na prática](#modelagem-de-ameaças-na-prática)  
4.1.2 [pytm](#pytm)  
4.1.3 [Threat Dragon](#threat-dragon)  
4.1.4 [Cornucopia](#cornucopia)  
4.1.5 [LINDDUN GO](#linddun-go)  
4.1.6 [Toolkit para Modelagem de Ameaças](#toolkit-para-modelagem-de-ameaças)  
4.2 [Lista de verificação para aplicação web](#lista-de-verificação-para-aplicação-web)  
4.2.1 [Defina Requisitos de Segurança](#defina-requisitos-de-segurança)  
4.2.2 [Utilize Frameworks e Bibliotecas de Segurança](#utilize-frameworks-e-bibliotecas-de-segurança)  
4.2.3 [Proteja Acesso ao Banco de Dados](#proteja-acesso-ao-banco-de-dados)  
4.2.4 [Codifique e Escape Dados](#codifique-e-escape-dados)  
4.2.5 [Valide todas as entradas](#valide-todas-as-entradas)  
4.2.6 [Implemente Identidade Digital](#implemente-identidade-digital)  
4.2.7 [Imponha Controles de Accesso](#imponha-controles-de-accesso)  
4.2.8 [Proteja Dados em Todos os Lugares](#proteja-dados-em-todos-os-lugares)  
4.2.9 [Implemente Registro e Monitoramento de Segurança](#implemente-registro-e-monitoramento-de-segurança)  
4.2.10 [Trate todos os Errors e Exceções](#trate todos-os-errors-e-exceções)  
4.3 [MAS Lista de verificação](#mas-lista-de-verificação)  

5 **[Implementação](#implementação)**  
5.1 [Documentação](#documentação)  
5.1.1 [Top 10 Controles Proativos](#top-controles-proativos)  
5.1.2 [GoSCP (Práticas de Codificação Segura em Go)](#goscp-práticas-de-codificação-segura-em-go)  
5.1.3 [Série de Folha de dicas](#série-de-folha-de-dicas)  
5.2 [Dependências](#dependências)
5.2.1 [Dependency-Check](#dependency-check)  
5.2.2 [Dependency-Track](#dependency-track)  
5.2.3 [CycloneDX](#cyclonedx)  
5.3 [Bibliotecas Seguras](#bibliotecas_seguras)  
5.3.1 [ESAPI](#esapi)  
5.3.2 [CSRFGuard](#csrfguard)  
5.3.3 [OSHP](#oshp)  
5.4 [MASWE](#maswe)

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
11.1.2 [ASVS (Padrão de Verificação de Segurança de Aplicações)](#application-security-verification-standard)  
11.1.3 [MAS (Segurança de Aplicativos Móveis)](#mobile-application-security)  
11.2 [BLT (Ferramenta de registro de bugs)](#bug-logging-tool)  

12 **[Appendices](#appendices)**  
12.1 [O que fazer e o que não fazer na Implementação](#implementation-dos-and-donts)  
12.1.1 [Segurança de containers](#container-security)  
12.1.2 [Codificação segura](#secure-coding)  
12.1.3 [Práticas de criptografia](#cryptographic-practices)  
12.1.4 [Spoofing de Aplicação](#application-spoofing)  
12.1.5 [Política de Segurança de Conteúdo (CSP)](#content-security-policy)  
12.1.6 [Tratamento de erros e exceções](#exception-and-error-handling)  
12.1.7 [Gerenciamento de arquivos](#file-management)  
12.1.8 [Gerenciamento de memória](#memory-management)  
12.2 [O que fazer e o que não fazer na Verificação](#verification-dos-and-donts)  
12.2.1 [Ambiente seguro](#secure-environment)  
12.2.2 [Hardening de sistemas](#system-hardening)  
12.2.3 [Software de Código Aberto](#open-source-software)  
