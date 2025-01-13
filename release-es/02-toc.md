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

3 **[Requerimientos](#requerimientos)**  
3.1 [Requerimientos en la práctica](#requerimientos-en-la-práctica)  
3.2 [Perfil de riesgo](#perfil de riesgo)  
3.3 [OpenCRE](#opencre)  
3.4 [SecurityRAT](#securityrat)  
3.5 [ASVS requerimientos](#asvs-requerimientos)  
3.6 [MAS requerimientos](#mas-requerimientos)  
3.7 [SKF requerimientos](#skf-requerimientos)  

4 **[Diseño](#diseño)**  
4.1 [Modelado de amenazas](#modelado-de-amenazas)  
4.1.1 [Modelado de amenazas en la práctica](#modelado-de-amenazas-en-la-práctica)  
4.1.2 [pytm](#pytm)  
4.1.3 [Threat Dragon](#threat-dragon)  
4.1.4 [Cornucopia](#cornucopia)  
4.1.5 [LINDDUN GO](#linddun-go)  
4.1.6 [Kit de herramientas de modelado de amenazas](#kit-de-herramientas-de-modelado-de- amenazas)  
4.2 [Lista de verificación de aplicaciones web](#lista-de-verificación-de-aplicaciones-web)  
4.2.1 [Definir requisitos de seguridad](#definir-requisitos-de-seguridad)  
4.2.2 [Aprovechar los frameworks y librerías](#aprovechar-los-frameworks-y-librerías)  
4.2.3 [Asegurar el acceso a la base de datos](#asegurar-el-acceso-a-la-base-de-datos)  
4.2.4 [Codificar y escapar caracteres especiales en datos](#codificar-y-escapar-caracteres-especiales-en-datos)  
4.2.5 [Validar todas las entradas](#validar-todas-las-entradas)  
4.2.6 [Implementar identidad digital](#implementar-identidad-digital)  
4.2.7 [Hacer respetar los controles de acceso](#hacer-respetar-los-controles-de-acceso)  
4.2.8 [Proteger los datos en todas partes](#proteger-los-datos-en-todas-partes)  
4.2.9 [Implementar registro y monitoreo](#implementar-registro-y-monitoreo)  
4.2.10 [Manejar todos los errores y excepciones](#cmanejar-todos-los-errores-y-excepciones)  
4.3 [MAS lista de verificación](#mas-lista-de-verificación)  

5 **[Implementación](#implementación)**  
5.1 [Documentación](#documentación)  
5.1.1 [Los Top 10 controles proactivos](#los-Top-10-controles-proactivos)  
5.1.2 [GoSCP (Prácticas de codificación seguras de Go)](#goscp-prácticas-de-codificación-seguras-de-go)  
5.1.3 [Serie de hojas de referencia](#cheatsheet-series)  
5.2 [Dependencias](#dependencias)
5.2.1 [Dependency-Check](#dependency-check)  
5.2.2 [Dependency-Track](#dependency-track)  
5.2.3 [CycloneDX](#cyclonedx)  
5.3 [Librerías seguras](#librerías-seguras)  
5.3.1 [ESAPI](#esapi)  
5.3.2 [CSRFGuard](#csrfguard)  
5.3.3 [OSHP](#oshp)  
5.4 [MASWE](#maswe)  

6 **[Verificación](#verificación)**  
6.1 [Guías](#guías)  
6.1.1 [WSTG](#wstg)  
6.1.2 [MASTG](#mastg)  
6.1.3 [ASVS](#asvs)  
6.2 [Herramientas](#herramientas)  
6.2.1 [DAST](#dast)  
6.2.2 [Amass](#amass)  
6.2.3 [OWTF](#owtf)  
6.2.4 [Nettacker](#nettacker)  
6.2.5 [OSHP verificación](#oshp-verificación)  
6.3 [Frameworks](#frameworks)  
6.3.1 [SecureCodeBox](#securecodebox)  
6.4 [Gestión de vulnerabilidades](#gestión-de-vulnerabilidades)  
6.4.1 [DefectDojo](#defectdojo)  

7 **[Capacitación y Educación](#capacitación-y-educación)**  
7.1 [Aplicaciones vulnerables](#aplicaciones-vulnerables)  
7.1.1 [Juice Shop](#juice-shop)  
7.1.2 [WebGoat](#webgoat)  
7.1.3 [PyGoat](#pygoat)  
7.1.4 [Security Shepherd](#security-shepherd)  
7.2 [Secure Coding Dojo](#secure-coding-dojo)  
7.3 [SKF capacitación](#skf-capacitación)  
7.4 [SamuraiWTF](#samuraiwtf)  
7.5 [Proyecto OWASP Top 10](#proyecto-owasp-top-10)  
7.6 [Mobile Top 10](#mobile-top-10)  
7.7 [API Top 10](#api-top-10)  
7.8 [WrongSecrets](#wrongsecrets)  
7.9 [OWASP Snakes and Ladders](#owasp-snakes-and-ladders)  

8 **[Desarrollo de cultura y maduración de procesos](#desarrollo-de-cultura-y-maduración-de-procesos)**  
8.1 [Cultura de seguridad](#cultura-de-seguridad)  
8.2 [Defensores de Seguridad](#defensores-de-seguridad)  
8.2.1 [Programa de Defensores de seguridad](#programa-de-defensores-de-seguridad)  
8.2.2 [Security Champions Guide](#security-champions-guide)  
8.2.3 [Security Champions Playbook](#security-champions-playbook)  
8.3 [SAMM](#samm)  
8.4 [ASVS procesos](#asvs-procesos)  
8.5 [MAS procesos](#mas-procesos)  

9 **[Operaciones](#operaciones)**  
9.1 [Directriz DevSecOps](#directriz-devsecops)  
9.2 [Coraza WAF](#coraza-waf)  
9.3 [ModSecurity WAF](#modsecurity-waf)  
9.4 [OWASP CRS](#owasp-crs)  

10 **[Métricas](#métricas)**  

11 **[Análisis de brechas de seguridad](#análisis-de-brechas-de-seguridad)**  
11.1 [Guías](#guías)  
11.1.1 [SAMM análisis](#samm-análisis)  
11.1.2 [ASVS análisis](#asvs-análisis)  
11.1.3 [MAS análisis](#mas-análisis)  
11.2 [BLT](#blt)  

12 **[Apéndices](#apéndices)**  
12.1 [Qué hacer y qué no hacer en la implementación](#qué-hacer-y-qué-no-hacer-en-la-implementación)  
12.1.1 [Seguridad de Contenedores](#seguridad-de-contenedores)  
12.1.2 [Codificación segura](#codificación-segura)  
12.1.3 [Prácticas criptográficas](#prácticas-criptográficas)  
12.1.4 [Suplantación de aplicaciones](#suplantación-de-aplicaciones)  
12.1.5 [Política de seguridad de contenido (CSP)](#política-de-seguridad-de-contenido-csp)  
12.1.6 [Manejo de excepciones y errores](#manejo-de-excepciones-y-errores)  
12.1.7 [Administración de archivos](#administración-de-archivos)  
12.1.8 [Administración de memoria](#administración-de-memoria)  
12.2 [Qué hacer y qué no hacer en la verificación](#verification-dos-and-donts)  
12.2.1 [Entorno seguro](#entorno-seguro)  
12.2.2 [Refuerzo de seguridad del sistema](#refuerzo-de-seguridad-del-sistema)  
12.2.3 [Software de código abierto](#software-de-código-abierto)  

\newpage
