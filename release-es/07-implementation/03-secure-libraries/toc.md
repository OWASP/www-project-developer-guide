---

title: Implementación de Librerías seguras
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Roxana Calderon
document: Guía del Desarrollador OWASP
order: 47300
permalink: /release-es/implementación/librerías_seguras/

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

![Logotipo de la Guía del Desarrollador](../../../assets/images/dg_logo_bbd.png "Guía del Desarrollador OWASP"){: .image-right }

### 5.3 Librerías seguras

El uso de librerías seguras es parte de la gestión tecnológica que ayuda a cumplir los requisitos de seguridad.
Las librerías estándar permiten la adopción de patrones de diseño comunes y soluciones de seguridad,
y proporcionan tecnologías y marcos estandarizados que pueden utilizarse en diferentes aplicaciones.

La [Gestión Tecnológica][sammdsatm] para las aplicaciones de software es descrita por SAMM como una actividad
dentro de la práctica de seguridad [Arquitectura de Seguridad][sammdsa] de SAMM,
que a su vez es parte de la función de negocio [Diseño][sammd].

Secciones:

5.3.1 [ESAPI](01-esapi.md)  
5.3.2 [CSRFGuard](02-csrf-guard.md)  
5.3.3 [OSHP](03-secure-headers.md)  

----
Traducción de versión [original en inglés][release0703].

La Guía del Desarrollador de OWASP es un esfuerzo comunitario; si hay algo que necesita cambiarse,
[envía un issue][issue0703] o [edita en GitHub][edit0703].

[release0703]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/07-implementation/03-secure-libraries/toc.md
[edit0703]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/07-implementation/03-secure-libraries/toc.md
[issue0703]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2007-implementation/03-secure-libraries/00-toc
[sammd]: https://owaspsamm.org/model/design/
[sammdsa]: https://owaspsamm.org/model/design/secure-architecture/
[sammdsatm]: https://owaspsamm.org/model/design/secure-architecture/stream-b/

/newpage