---

title: Herramientas de Verificación
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Roxana Calderon
document: Guía del Desarrollador OWASP
order:

---

{% include breadcrumb.html %}

![Logo de guía del desarrollador](../../../assets/images/dg_logo_bbd.png "Guía del Desarrollador OWASP"){height=180px}

### 6.2 Herramientas de verificación

[Verificación][sammv] es una de las funciones de negocio descritas por [OWASP SAMM][samm].

La actividad de [Testeo de Seguridad][sammvst] de SAMM describe el uso tanto de pruebas de seguridad automatizadas como pruebas de seguridad manuales por expertos para descubrir defectos de seguridad.
Estas pruebas de seguridad deben ser automatizadas como parte de los procesos de desarrollo, construcción y despliegue;
y pueden ser complementadas con pruebas manuales de seguridad de penetración de forma regular.

Las herramientas automatizadas de pruebas de seguridad son rápidas y escalan bien para numerosas aplicaciones,
mientras que las pruebas de seguridad manuales de componentes de alto riesgo requieren un buen conocimiento de la aplicación y su lógica de negocio.

Secciones:

6.2.1 [Herramientas DAST](#dast-tools)  
6.2.2 [Amass](#amass)  
6.2.3 [OWTF](#owtf)  
6.2.4 [Nettacker](#nettacker)  
6.2.5 [Verificación OSHP](#oshp-verification)  

----
Traducción de versión [original en inglés][release0401].

La Guía del Desarrollador de OWASP es un esfuerzo comunitario; si hay algo que necesita cambios, [envía un issue][issue0820].

[release0820]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/08-verification/02-tools/toc.md
[issue0820]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2008-verification/02-tools/00-toc
[samm]: https://owaspsamm.org/about/
[sammv]: https://owaspsamm.org/model/verification/
[sammvst]: https://owaspsamm.org/model/verification/security-testing/

\newpage
