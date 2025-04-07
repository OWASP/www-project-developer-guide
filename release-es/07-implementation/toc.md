---

title: Implementación
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Roxana Calderon
document: Guía del Desarrollador OWASP
order: 47000
permalink: /release-es/implementación/

---

{% include breadcrumb.html %}

<style type="text/css">
.image-right {
  height: 180px;
  display: block;
  margin-left: auto;
  margin-right: auto;
  float: right;
}
</style>

![Logo de la guía del desarrollador](../../assets/images/dg_logo.png "Guía del Desarrollador OWASP"){: .image-right }

## 5. Implementación

La función de negocio [Implementación][sammi] está descrita
por el [Modelo de Madurez de Aseguramiento de Software][sammm] (SAMM) de OWASP.
La Implementación se centra en los procesos y actividades relacionadas con la manera en que una organización
construye y despliega componentes de software y sus defectos relacionados.
Las actividades de Implementación tienen el mayor impacto en la vida diaria de los desarrolladores,
y un objetivo importante de la Implementación es entregar software que funcione de manera confiable
con un mínimo de defectos.

La Implementación debe incluir prácticas de seguridad como:

* Construcción Segura
* Despliegue Seguro
* Gestión de Defectos

La Implementación es donde la aplicación/sistema comienza a tomar forma; se escribe el código fuente y se crean las pruebas.
La implementación de la aplicación sigue un ciclo de vida de desarrollo seguro, con seguridad incorporada desde el inicio.

La implementación utilizará un método seguro de control y almacenamiento del código fuente para cumplir
con los requisitos de seguridad del diseño.
El equipo de desarrollo se referirá a la documentación que aconseja sobre las mejores prácticas,
utilizarán bibliotecas seguras siempre que sea posible, además de verificar
y realizar seguimiento de las dependencias externas.

Gran parte de la habilidad de implementación proviene de la experiencia, y tener en cuenta los que se debe hacer
y lo que no se debe hacer
durante el desarrollo seguro es en sí misma una actividad de conocimiento importante.

Secciones:

5.1 [Documentación](01-documentation/toc.md)  
5.1.1 [Los 10 Principales Controles Proactivos](01-documentation/01-proactive-controls.md)  
5.1.2 [Prácticas de Codificación Segura en Go](01-documentation/02-go-scp.md)  
5.1.3 [Serie de Hojas de Referencia](01-documentation/03-cheatsheets.md)  
5.2 [Dependencias](02-dependencies/toc.md)  
5.2.1 [Dependency-Check](02-dependencies/01-dependency-check.md)  
5.2.2 [Dependency-Track](02-dependencies/02-dependency-track.md)  
5.2.3 [CycloneDX](02-dependencies/03-cyclonedx.md)  
5.3 [Bibliotecas Seguras](03-secure-libraries/toc.md)  
5.3.1 [ESAPI](03-secure-libraries/01-esapi.md)  
5.3.2 [CSRFGuard](03-secure-libraries/02-csrf-guard.md)  
5.3.3 [OSHP](03-secure-libraries/03-secure-headers.md)  
5.4 [MASWE](04-maswe.md)  

----
Traducción de versión [original en inglés][release0700].

La Guía del Desarrollador de OWASP es un esfuerzo comunitario; si hay algo que necesita cambiarse,
[envía un problema][issue0700] o [edita en GitHub][edit0700].release0700

[release0700]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/07-implementation/toc.md
[edit0700]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/07-implementation/toc.md
[issue0700]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2007-implementation/00-toc
[sammm]: https://owaspsamm.org/model/
[sammi]: https://owaspsamm.org/model/implementation/
