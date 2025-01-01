---

title: Tabla de contenido
layout: col-document
tags: OWASP Developer Guide
contributors: Roxana Calderon
document: OWASP Developer Guide
order: 42000
permalink: /release-es/

---

{% include breadcrumb.html %}

![Developer guide logo](../assets/images/dg_logo.png "OWASP Developer Guide"){: height="180px" }

### Guía del desarrollador OWASP

#### Una guía para dessarrollar aplicaciones y servicios web seguros

1 **[Introducción](03-introduction.md)**

2 **[Fundamentos](04-foundations/toc.md)**  
2.1 [Fundamentos de Seguridad](04-foundations/01-security-fundamentals.md)  
2.2 [Desarrollo e integración Segura](04-foundations/02-secure-development.md)  
2.3 [Principios de Seguridad](04-foundations/03-security-principles.md)  
2.4 [Principios de Criptografía](04-foundations/04-crypto-principles.md)  
2.5 [Top 10 de OWASP](04-foundations/05-top-ten.md)  

3 **[Requerimientos](05-requirements/toc.md)**  
3.1 [Requerimientos en la práctica](05-requirements/01-requirements.md)  
3.2 [Perfil de riesgo](05-requirements/02-risk.md)  
3.3 [OpenCRE](05-requirements/03-int-stand.md)  
3.4 [SecurityRAT](05-requirements/04-security-rat.md)  
3.5 [Estandard de Verificación de Securidad de Aplicaciones](05-requirements/05-asvs.md)  
3.6 [Seguridad de aplicaciones móviles](05-requirements/06-mas.md)  
3.7 [Framework de Conocimiento de Seguridad](05-requirements/07-skf.md)  

4 **[Diseño](06-design/toc.md)**  
4.1 [Modelado de amenazas](06-design/01-threat-modeling/toc.md)  
4.1.1 [Modelado de amenazas en la práctica](06-design/01-threat-modeling/01-threat-modeling.md)  
4.1.2 [pytm](06-design/01-threat-modeling/02-pytm.md)  
4.1.3 [Threat Dragon](06-design/01-threat-modeling/03-threat-dragon.md)  
4.1.4 [Cornucopia](06-design/01-threat-modeling/04-cornucopia.md)  
4.1.5 [LINDDUN GO](06-design/01-threat-modeling/05-linddun-go.md)  
4.1.6 [Kit de herramientas de modelado de amenazas](06-design/01-threat-modeling/06-toolkit.md)  
4.2 [Lista de verificación de aplicaciones web](06-design/02-web-app-checklist/toc.md)  
4.2.1 [Definir requisitos de seguridad](06-design/02-web-app-checklist/01-define-security-requirements.md)  
4.2.2 [Aprovechar los frameworks y librerías](06-design/02-web-app-checklist/02-frameworks-libraries.md)  
4.2.3 [Asegurar el acceso a la base de datos](06-design/02-web-app-checklist/03-secure-database-access.md)  
4.2.4 [Codificar y escapar caracteres especiales en datos](06-design/02-web-app-checklist/04-encode-escape-data.md)  
4.2.5 [Validar todas las entradas](06-design/02-web-app-checklist/05-validate-inputs.md)  
4.2.6 [Implementar identidad digital](06-design/02-web-app-checklist/06-digital-identity.md)  
4.2.7 [Hacer respetar los controles de acceso](06-design/02-web-app-checklist/07-access-controls.md)  
4.2.8 [Proteger los datos en todas partes](06-design/02-web-app-checklist/08-protect-data.md)  
4.2.9 [Implementar registro y monitoreo de seguridad](06-design/02-web-app-checklist/09-logging-monitoring.md)  
4.2.10 [Manejar todos los errores y excepciones](06-design/02-web-app-checklist/10-handle-errors-exceptions.md)  
4.3 [Lista de verificación de aplicaciones móviles](06-design/03-mas-checklist.md)  

5 **[Implementación](07-implementation/toc.md)**  
5.1 [Documentación](07-implementation/01-documentation/toc.md)  
5.1.1 [Los Top 10 controles proactivos](07-implementation/01-documentation/01-proactive-controls.md)  
5.1.2 [Prácticas de codificación seguras de Go](07-implementation/01-documentation/02-go-scp.md)  
5.1.3 [Serie de hojas de referencia](07-implementation/01-documentation/03-cheatsheets.md)  
5.2 [Dependencias](07-implementation/02-dependencies/toc.md)  
5.2.1 [Dependency-Check](07-implementation/02-dependencies/01-dependency-check.md)  
5.2.2 [Dependency-Track](07-implementation/02-dependencies/02-dependency-track.md)  
5.2.3 [CycloneDX](07-implementation/02-dependencies/03-cyclonedx.md)  
5.3 [Librerías seguras](07-implementation/03-secure-libraries/toc.md)  
5.3.1 [Librería de API de seguridad empresarial](07-implementation/03-secure-libraries/01-esapi.md)  
5.3.2 [Librería CSRFGuard](07-implementation/03-secure-libraries/02-csrf-guard.md)  
5.3.3 [Proyecto OWASP Secure Headers](07-implementation/03-secure-libraries/03-secure-headers.md)  
5.4 [Mobile application weakness enumeration](07-implementation/04-maswe.md)  

6 **[Verificación](08-verification/toc.md)**  
6.1 [Guías](08-verification/01-guides/toc.md)  
6.1.1 [Guía de testeo de seguridad web](08-verification/01-guides/01-wstg.md)  
6.1.2 [Guía de testeo MAS](08-verification/01-guides/02-mastg.md)  
6.1.3 [Estándar de verificación de seguridad de aplicaciones](08-verification/01-guides/03-asvs.md)  
6.2 [Herramientas](08-verification/02-tools/toc.md)  
6.2.1 [DAST tools](08-verification/02-tools/01-dast.md)  
6.2.2 [Amass](08-verification/02-tools/02-amass.md)  
6.2.3 [Framework Offensive Web Testing](08-verification/02-tools/03-owtf.md)  
6.2.4 [Nettacker](08-verification/02-tools/04-nettacker.md)  
6.2.5 [Proyecto OWASP Secure Headers](08-verification/02-tools/05-secure-headers.md)  
6.3 [Frameworks](08-verification/03-frameworks/toc.md)  
6.3.1 [SecureCodeBox](08-verification/03-frameworks/01-secure-codebox.md)  
6.4 [Gestión de vulnerabilidades](08-verification/04-vulnerability-management/toc.md)  
6.4.1 [DefectDojo](08-verification/04-vulnerability-management/01-defectdojo.md)  

7 **[Capacitación y Educación](09-training-education/toc.md)**  
7.1 [Aplicaciones vulnerables](09-training-education/01-vulnerable-apps/toc.md)  
7.1.1 [Juice Shop](09-training-education/01-vulnerable-apps/01-juice-shop.md)  
7.1.2 [WebGoat](09-training-education/01-vulnerable-apps/02-webgoat.md)  
7.1.3 [PyGoat](09-training-education/01-vulnerable-apps/03-pygoat.md)  
7.1.4 [Security Shepherd](09-training-education/01-vulnerable-apps/04-security-shepherd.md)  
7.2 [Secure Coding Dojo](09-training-education/02-secure-coding-dojo.md)  
7.3 [Security Knowledge Framework](09-training-education/03-skf.md)  
7.4 [SamuraiWTF](09-training-education/04-samurai-wtf.md)  
7.5 [Proyecto OWASP Top 10](09-training-education/05-top-ten.md)  
7.6 [Mobile Top 10](09-training-education/06-mobile-top-ten.md)  
7.7 [API Top 10](09-training-education/07-api-top-ten.md)  
7.8 [WrongSecrets](09-training-education/08-wrongsecrets.md)  
7.9 [OWASP Snakes and Ladders](09-training-education/09-snakes-ladders.md)  

8 **[Desarrollo de cultura y maduración de procesos](10-culture-process/toc.md)**  
8.1 [Cultura de seguridad](10-culture-process/01-security-culture.md)  
8.2 [Defensores de Seguridad](10-culture-process/02-security-champions/toc.md)  
8.2.1 [Programa de Defensores de seguridad](10-culture-process/02-security-champions/01-security-champions-program.md)  
8.2.2 [Guía de Defensores de seguridad](10-culture-process/02-security-champions/02-security-champions-guide.md)  
8.2.3 [Manual de Defensores de seguridad](10-culture-process/02-security-champions/03-security-champions-playbook.md)  
8.3 [Modelo de madurez de garantía de software](10-culture-process/03-samm.md)  
8.4 [Estándar de verificación de seguridad de aplicaciones](10-culture-process/04-asvs.md)  
8.5 [Seguridad de aplicaciones móviles](10-culture-process/05-mas.md)  

9 **[Operaciones](11-operations/toc.md)**  
9.1 [Directriz DevSecOps](11-operations/01-devsecops.md)  
9.2 [Firewall de aplicaciones web Coraza](11-operations/02-coraza.md)  
9.3 [Firewall de aplicaciones web ModSecurity](11-operations/03-modsecurity.md)  
9.4 [OWASP CRS](11-operations/04-crs.md)  

10 **[Métricas](12-metrics/toc.md)**  

11 **[Análisis de brechas de seguridad](13-security-gap-analysis/01-guides/toc.md)**  
11.1 [Guías](13-security-gap-analysis/01-guides/toc.md)  
11.1.1 [Modelo de madurez de garantía de software](13-security-gap-analysis/01-guides/01-samm.md)  
11.1.2 [Estándar de verificación de seguridad de aplicaciones](13-security-gap-analysis/01-guides/02-asvs.md)  
11.1.3 [Seguridad de aplicaciones móviles](13-security-gap-analysis/01-guides/03-mas.md)  
11.2 [Herramienta de registro de errores](13-security-gap-analysis/02-blt.md)  

12 **[Apéndices](14-appendices/toc.md)**  
12.1 [Qué hacer y qué no hacer en la implementación](14-appendices/01-implementation-dos-donts/toc.md)  
12.1.1 [Seguridad de Contenedores](14-appendices/01-implementation-dos-donts/01-container-security.md)  
12.1.2 [Codificación segura](14-appendices/01-implementation-dos-donts/02-secure-coding.md)  
12.1.3 [Prácticas criptográficas](14-appendices/01-implementation-dos-donts/03-cryptographic-practices.md)  
12.1.4 [Suplantación de aplicaciones](14-appendices/01-implementation-dos-donts/04-application-spoofing.md)  
12.1.5 [Política de seguridad de contenido (CSP)](14-appendices/01-implementation-dos-donts/05-content-security-policy.md)  
12.1.6 [Manejo de excepciones y errores](14-appendices/01-implementation-dos-donts/06-exception-error-handling.md)  
12.1.7 [Administración de archivos](14-appendices/01-implementation-dos-donts/07-file-management.md)  
12.1.8 [Administración de memoria](14-appendices/01-implementation-dos-donts/08-memory-management.md)  
12.2 [Qué hacer y qué no hacer en la verificación](14-appendices/02-verification-dos-donts/toc.md)  
12.2.1 [Entorno seguro](14-appendices/02-verification-dos-donts/01-secure-environment.md)  
12.2.2 [Refuerzo de seguridad del sistema](14-appendices/02-verification-dos-donts/02-system-hardening.md)  
12.2.3 [Software de código abierto](14-appendices/02-verification-dos-donts/03-open-source-software.md)  
