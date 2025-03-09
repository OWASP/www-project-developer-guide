---

title: Requisitos
layout: col-document
tags: Guía del desarrollador OWASP
contributors: Jon Gadsden, Andreas Happe, Roxana Calderon
document: Guía del desarrollador OWASP
order: 45000
permalink: /release-es/requirements/

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

![Logo de la guía del desarrollador](../../assets/images/dg_logo.png "Guía del desarrollador OWASP"){: .image-right }

## 3. Requisitos

Los requisitos de seguridad también proporcionan una base de funcionalidad de seguridad minuciosamente verificada para una aplicación.
En lugar de crear un enfoque personalizado de seguridad para cada aplicación,
los requisitos de seguridad estándar permiten a los desarrolladores reutilizar la definición de controles de seguridad y mejores prácticas;
esos mismos requisitos de seguridad verificados proporcionan soluciones para problemas de seguridad que han ocurrido en el pasado.

La importancia de comprender los requisitos clave de seguridad se describe en la práctica de [Requisitos de Seguridad][sammdsr]
que forma parte de la sección de función empresarial [Diseño][sammd] dentro del [modelo SAMM][samm] de OWASP.
Idealmente, los requisitos de seguridad de software estructurados están disponibles dentro de un marco de requisitos de seguridad,
y estos son utilizados tanto por los equipos de desarrolladores como por los equipos de producto.
Además, los proveedores de la organización deben cumplir con los requisitos de seguridad;
incorporar la seguridad en los acuerdos con proveedores para garantizar el cumplimiento de los requisitos de seguridad organizacionales.

En resumen, los requisitos de seguridad existen para prevenir la repetición de fallos de seguridad pasados.

Secciones:

3.1 [Requisitos en la práctica](01-requirements.md)  
3.2 [Perfil de riesgo](02-risk.md)  
3.3 [OpenCRE](03-opencre.md)  
3.4 [SecurityRAT](04-security-rat.md)  
3.5 [Requisitos ASVS](05-asvs.md)  
3.6 [Requisitos MAS](06-mas.md)  
3.7 [Requisitos SKF](07-skf.md)  

----
Traducción de versión [original en inglés][release0500].

La Guía del Desarrollador de OWASP es un esfuerzo comunitario; si hay algo que necesita cambiar
entonces [cree un issue][issue0500] o [edítelo en GitHub][edit0500].

[release0500]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/05-requirements/toc.md
[edit0500]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/05-requirements/toc.md
[issue0500]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2005-requirements/00-toc
[samm]: https://owaspsamm.org/about/
[sammd]: https://owaspsamm.org/model/design/
[sammdsr]: https://owaspsamm.org/model/design/security-requirements/
