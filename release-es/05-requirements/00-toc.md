---

title: Requisitos
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Roxana Calderon, Andreas Happe
document: Guía del Desarrollador OWASP
order:
permalink:

---

{% include breadcrumb.html %}

![Logo de la guía del desarrollador](../../assets/images/dg_logo.png "Guía del Desarrollador OWASP"){height=180px}

## 3. Requisitos

Los requisitos de seguridad también proporcionan una base de funcionalidad de seguridad minuciosamente verificada
para una aplicación.
En lugar de crear un enfoque personalizado de seguridad para cada aplicación,
los requisitos de seguridad estándar permiten a los desarrolladores reutilizar
la definición de controles de seguridad y mejores prácticas;
esos mismos requisitos de seguridad verificados proporcionan soluciones para problemas de seguridad
que han ocurrido en el pasado.

La importancia de comprender los requisitos clave de seguridad se describe en
la práctica de [Requisitos de Seguridad][sammdsr]
que forma parte de la sección de función empresarial [Diseño][sammd] dentro del [modelo SAMM][samm] de OWASP.
Idealmente, los requisitos de seguridad de software estructurados están disponibles dentro de
un marco de requisitos de seguridad,
y estos son utilizados tanto por los equipos de desarrolladores como por los equipos de producto.
Además, los proveedores de la organización deben cumplir con los requisitos de seguridad;
incorporar la seguridad en los acuerdos con proveedores para garantizar el cumplimiento de
los requisitos de seguridad organizacionales.

En resumen, los requisitos de seguridad existen para prevenir la repetición de fallos de seguridad pasados.

Secciones:

3.1 [Requisitos en la práctica](#requisitos-en-la-práctica)  
3.2 [Perfil de riesgo](#perfil-de-riesgo)  
3.3 [OpenCRE](#opencre)  
3.4 [SecurityRAT](#security-rat)  
3.5 [Requisitos ASVS](#requisitos-asvs)  
3.6 [Requisitos MAS](#requisitos-mas)  
3.7 [Requisitos SKF](#requisitos-skf)  

----
Traducción de versión [original en inglés][release0500].
La Guía de Desarrollador OWASP es un esfuerzo comunitario; si hay algo que necesite cambios, [cree un issue][issue0500].

[release0500]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/05-requirements/00-toc.md
[issue0500]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2005-requirements/00-toc
[samm]: https://owaspsamm.org/about/
[sammd]: https://owaspsamm.org/model/design/
[sammdsr]: https://owaspsamm.org/model/design/security-requirements/
