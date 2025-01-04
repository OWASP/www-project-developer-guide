---

title: Design
layout: col-document
tags: Guia do Desenvolvedor do OWASP
contributors:
document: Guia do Desenvolvedor do OWASP
order:

---

{% include breadcrumb.html %}

![WIP logo](../../../assets/images/dg_wip.png "Trabalho em andamento"){height=180px}

## 4. Design

Não há tradução para esta página, consulte a [versão original em inglês][release0600].

Sections:

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

----

[release0600]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/toc.md
