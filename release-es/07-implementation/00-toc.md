---

title: Implementación
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Roxana Calderon
document: Guía del Desarrollador OWASP
order:

---

{% include breadcrumb.html %}

![Logo de la guía del desarrollador](../../assets/images/dg_logo.png "Guía del Desarrollador OWASP"){height=180px}

## 5. Implementación

La función de negocio [Implementación][sammi] está descrita por el [Modelo de Madurez de Aseguramiento de Software][sammm] (SAMM) de OWASP.
La Implementación se centra en los procesos y actividades relacionadas con la manera en que una organización
construye y despliega componentes de software y sus defectos relacionados.
Las actividades de Implementación tienen el mayor impacto en la vida diaria de los desarrolladores,
y un objetivo importante de la Implementación es entregar software que funcione de manera confiable con un mínimo de defectos.

La Implementación debe incluir prácticas de seguridad como:

* Construcción Segura
* Despliegue Seguro
* Gestión de Defectos

La Implementación es donde la aplicación/sistema comienza a tomar forma; se escribe el código fuente y se crean las pruebas.
La implementación de la aplicación sigue un ciclo de vida de desarrollo seguro, con seguridad incorporada desde el inicio.

La implementación utilizará un método seguro de control y almacenamiento del código fuente para cumplir con los requisitos de seguridad del diseño.
El equipo de desarrollo se referirá a la documentación que aconseja sobre las mejores prácticas,
utilizará bibliotecas seguras siempre que sea posible, además de verificar y realizar seguimiento de las dependencias externas.

Gran parte de la habilidad de implementación proviene de la experiencia, y tener en cuenta lo que se debe hacer y lo que no se debe hacer
durante el desarrollo seguro es en sí misma una actividad de conocimiento importante.

Secciones:

5.1 [Documentación](#documentation)  
5.1.1 [Top 10 Controles Proactivos](#top-proactive-controls)  
5.1.2 [Prácticas de Codificación Segura en Go](#go-secure-coding-practices)  
5.1.3 [Serie de Hojas de Referencia](#cheatsheet-series)  
5.2 [Dependencias](#dependencies)
5.2.1 [Dependency-Check](#dependency-check)  
5.2.2 [Dependency-Track](#dependency-track)  
5.2.3 [CycloneDX](#cyclonedx)  
5.3 [Bibliotecas Seguras](#secure-libraries)  
5.3.1 [ESAPI](#esapi)  
5.3.2 [CSRFGuard](#csrfguard)  
5.3.3 [OSHP](#oshp)  
5.4 [MASWE](#maswe)  

----
Traducción de versión [original en inglés][release0700].

La Guía del Desarrollador de OWASP es un esfuerzo comunitario; si hay algo que necesita cambiarse, [cree un issue][issue0700].

[release0700]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/07-implementation/toc.md
[issue0700]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2007-implementation/00-toc
[sammm]: https://owaspsamm.org/model/
[sammi]: https://owaspsamm.org/model/implementation/

\newpage