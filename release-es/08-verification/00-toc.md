---

title: Verificación
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Roxana Calderon
document: Guía del Desarrollador OWASP
order:

---

{% include breadcrumb.html %}

![Logotipo de la guía del desarrollador](../../assets/images/dg_logo.png "Guía del Desarrollador OWASP"){height=180px}

## 6. Verificación

[Verificación][sammv] es una de las funciones de negocio descritas por [OWASP SAMM][samm].

La verificación se centra en los procesos y actividades relacionados con cómo una organización comprueba
y prueba los artefactos producidos durante el desarrollo de software.
Esto típicamente incluye trabajo de aseguramiento de calidad como pruebas, y también incluye otras actividades de revisión y evaluación.

Las actividades de verificación deberían incluir:

* Evaluación, validación y mitigación de la arquitectura
* Pruebas basadas en requisitos
* Verificación de controles de seguridad y pruebas de mal uso/abuso
* Pruebas de seguridad automatizadas y establecimiento de líneas base
* Pruebas de seguridad manuales y pruebas de penetración

Estas actividades están respaldadas por:

* Guías de seguridad
* Herramientas de prueba
* Frameworks de prueba
* Gestión de vulnerabilidades
* Listas de verificación

La verificación es una actividad central en el ciclo de vida de desarrollo de software seguro.
Consulte la sección del proyecto [Cultura de Seguridad][culturetest] para los diversos tipos de pruebas de seguridad.

Secciones:

6.1 [Guías](#verification-guides)  
6.1.1 [WSTG](#wstg)  
6.1.2 [MASTG](#mastg)  
6.1.3 [ASVS](#asvs)  
6.2 [Herramientas](#verification-tools)  
6.2.1 [Herramientas DAST](#dast-tools)  
6.2.2 [Amass](#amass)  
6.2.3 [OWTF](#owtf)  
6.2.4 [Nettacker](#nettacker)  
6.2.5 [Verificación OSHP](#oshp-verification)  
6.3 [Frameworks](#verification-frameworks)  
6.3.1 [secureCodeBox](#securecodebox)  
6.4 [Gestión de vulnerabilidades](#verification-vulnerability-management)  
6.4.1 [DefectDojo](#defectdojo)  

----
Traducción de versión [original en inglés][release0800].

La Guía del Desarrollador de OWASP es un esfuerzo comunitario; si hay algo que necesita cambios, [cree un issue][issue0800].

[release0800]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/08-verification/toc.md
[culturetest]: https://owasp.org/www-project-security-culture/stable/7-Security_Testing/
[issue0800]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2008-verification/00-toc
[samm]: https://owaspsamm.org/about/
[sammv]: https://owaspsamm.org/model/verification/

\newpage