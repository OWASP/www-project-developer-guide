---

title: Tabla de contenido
layout: col-document
tags: Guía del desarrollador OWASP
contributors: Roxana Calderon
document: Guía del desarrollador OWASP
order:
permalink:

---

{% include breadcrumb.html %}

## Tabla de contenido

1 **[Introducción](#introducción)**  

2 **[Fundamentos](#fundamentos)**  
2.1 [Fundamentos de Seguridad](#fundamentos-de-seguridad)  
2.2 [Desarrollo e integración Segura](#desarrollo-e-integración-segura)  
2.3 [Principios de Seguridad](#principios-de-seguridad)  
2.4 [Principios de Criptografía](#principios-de-criptografía)  
2.5 [OWASP Top 10](#owasp-top-ten)  

3 **[Requerimientos](#requirements)**  
3.1 [Requerimientos en la práctica](#requirements-in-practice)  
3.2 [Perfil de riesgo](#risk-profile)  
3.3 [OpenCRE](#opencre)  
3.4 [SecurityRAT](#security-rat)  
3.5 [Estandard de Verificación de Securidad de Aplicaciones](#application-security-verification-standard)  
3.6 [Seguridad de aplicaciones móviles](#mobile-application-security)  
3.7 [Framework de Conocimiento de Seguridad](#security-knowledge-framework)  

4 **[Diseño](#design)**  
4.1 [Modelado de amenazas](#threat-modeling)  
4.1.1 [Modelado de amenazas en la práctica](#threat-modeling-in-practice)  
4.1.2 [pytm](#pytm)  
4.1.3 [Threat Dragon](#threat-dragon)  
4.1.4 [Cornucopia](#cornucopia)  
4.1.5 [LINDDUN GO](#linddun-go)  
4.1.6 [Kit de herramientas de modelado de amenazas](#threat-modeling-toolkit)  
4.2 [Lista de verificación de aplicaciones web](#web-application-checklist)  
4.2.1 [Lista de verificación: Definir requisitos de seguridad](#checklist-define-security-requirements)  
4.2.2 [Lista de verificación: Aprovechar los frameworks y librerías](#checklist-leverage-security-frameworks-and-libraries)  
4.2.3 [Lista de verificación: Asegurar el acceso a la base de datos](#checklist-secure-database-access)  
4.2.4 [Lista de verificación: Codificar y escapar caracteres especiales en datos](#checklist-encode-and-escape-data)  
4.2.5 [Lista de verificación: Validar todas las entradas](#checklist-validate-all-inputs)  
4.2.6 [Lista de verificación: Implementar identidad digital](#checklist-implement-digital-identity)  
4.2.7 [Lista de verificación: Hacer respetar los controles de acceso](#checklist-enforce-access-controls)  
4.2.8 [Lista de verificación: Proteger los datos en todas partes](#checklist-protect-data-everywhere)  
4.2.9 [Lista de verificación: Implementar registro y monitoreo](#checklist-implement-security-logging-and-monitoring)  
4.2.10 [Lista de verificación: Manejar todos los errores y excepciones](#checklist-handle-all-errors-and-exceptions)  
4.3 [Lista de verificación de aplicaciones móviles](#mobile-application-checklist)  

5 **[Implementación](#implementation)**  
5.1 [Documentación](#documentation)  
5.1.1 [Los Top 10 controles proactivos](#top-proactive-controls)  
5.1.2 [Prácticas de codificación seguras de Go](#go-secure-coding-practices)  
5.1.3 [Serie de hojas de referencia](#cheatsheet-series)  
5.2 [Dependencias](#dependencies)
5.2.1 [Dependency-Check](#dependency-check)  
5.2.2 [Dependency-Track](#dependency-track)  
5.2.3 [CycloneDX](#cyclonedx)  
5.3 [Librerías seguras](#secure-libraries)  
5.3.1 [Librería de API de seguridad empresarial](#enterprise-security-api-library)  
5.3.2 [Librería CSRFGuard](#csrfguard-library)  
5.3.3 [Proyecto OWASP Secure Headers](#owasp-secure-headers-project)  
5.4 [Mobile application weakness enumeration](#mobile-application-weakness-enumeration)  

6 **[Verificación](#verification)**  
6.1 [Guías](#verification-guides)  
6.1.1 [Guía de testeo de seguridad web](#web-security-testing-guide)  
6.1.2 [Guía de testeo MAS](#mas-testing-guide)  
6.1.3 [Estándar de verificación de seguridad de aplicaciones](#application-security-verification-standard)  
6.2 [Herramientas](#verification-tools)  
6.2.1 [DAST tools](#dast-tools)  
6.2.2 [Amass](#amass)  
6.2.3 [Offensive Web Testing Framework](#offensive-web-testing-framework)  
6.2.4 [Nettacker](#nettacker)  
6.2.5 [Proyecto OWASP Secure Headers](#secure-headers-project)  
6.3 [Frameworks](#verification-frameworks)  
6.3.1 [SecureCodeBox](#securecodebox)  
6.4 [Gestión de vulnerabilidades](#verification-vulnerability-management)  
6.4.1 [DefectDojo](#defectdojo)  

7 **[Capacitación y Educación](#training-and-education)**  
7.1 [Aplicaciones vulnerables](#vulnerable-applications)  
7.1.1 [Juice Shop](#juice-shop)  
7.1.2 [WebGoat](#webgoat)  
7.1.3 [PyGoat](#pygoat)  
7.1.4 [Security Shepherd](#security-shepherd)  
7.2 [Secure Coding Dojo](#secure-coding-dojo)  
7.3 [Security Knowledge Framework](#security-knowledge-framework-training)  
7.4 [SamuraiWTF](#samuraiwtf)  
7.5 [Proyecto OWASP Top 10](#owasp-top-ten-project)  
7.6 [Mobile Top 10](#mobile-top-ten)  
7.7 [API Top 10](#api-top-ten)  
7.8 [WrongSecrets](#wrongsecrets)  
7.9 [OWASP Snakes and Ladders](#owasp-snakes-and-ladders)  

8 **[Desarrollo de cultura y maduración de procesos](#culture-building-and-process-maturing)**  
8.1 [Cultura de seguridad](#security-culture)  
8.2 [Defensores de Seguridad](#security-champions)  
8.2.1 [Programa de Defensores de seguridad](#security-champions-program)  
8.2.2 [Guía de Defensores de seguridad](#security-champions-guide)  
8.2.3 [Manual de Defensores de seguridad](#security-champions-playbook)  
8.3 [Modelo de madurez de garantía de software](#software-assurance-maturity-model)  
8.4 [Estándar de verificación de seguridad de aplicaciones](#application-security-verification-standard)  
8.5 [Seguridad de aplicaciones móviles](#mobile-application-security)  

9 **[Operaciones](#operations)**  
9.1 [Directriz DevSecOps](#devsecops-guideline)  
9.2 [Firewall de aplicaciones web Coraza](#coraza-web-application-firewall)  
9.3 [Firewall de aplicaciones web ModSecurity](#modsecurity-web-application-firewall)  
9.4 [OWASP CRS](#owasp-crs)  

10 **[Métricas](#metrics)**  

11 **[Análisis de brechas de seguridad](#security-gap-analysis)**  
11.1 [Guías](#security-gap-analysis-guides)  
11.1.1 [Modelo de madurez de garantía de software](#software-assurance-maturity-model)  
11.1.2 [Estándar de verificación de seguridad de aplicaciones](#application-security-verification-standard)  
11.1.3 [Seguridad de aplicaciones móviles](#mobile-application-security)  
11.2 [Herramienta de registro de errores](#bug-logging-tool)  

12 **[Apéndices](#appendices)**  
12.1 [Qué hacer y qué no hacer en la implementación](#implementation-dos-and-donts)  
12.1.1 [Seguridad de Contenedores](#container-security)  
12.1.2 [Codificación segura](#secure-coding)  
12.1.3 [Prácticas criptográficas](#cryptographic-practices)  
12.1.4 [Suplantación de aplicaciones](#application-spoofing)  
12.1.5 [Política de seguridad de contenido (CSP)](#content-security-policy)  
12.1.6 [Manejo de excepciones y errores](#exception-and-error-handling)  
12.1.7 [Administración de archivos](#file-management)  
12.1.8 [Administración de memoria](#memory-management)  
12.2 [Qué hacer y qué no hacer en la verificación](#verification-dos-and-donts)  
12.2.1 [Entorno seguro](#secure-environment)  
12.2.2 [Refuerzo de seguridad del sistema](#system-hardening)  
12.2.3 [Software de código abierto](#open-source-software)  

\newpage
