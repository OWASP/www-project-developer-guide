---

title: Requisitos
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Roxana Calderon, Jon Gadsden, Andreas Happe
document: Guía del Desarrollador OWASP
order:
permalink:

---

{% include breadcrumb.html %}

![Logo de la guía del desarrollador](../../assets/images/dg_logo.png "Guía del Desarrollador OWASP"){height=180px}

## 3. Requisitos

Los requisitos de seguridad son declaraciones de funcionalidad de seguridad que garantizan que se satisfagan las diferentes propiedades de seguridad de una aplicación de software.
Los requisitos de seguridad se derivan de estándares de la industria, leyes aplicables y un historial de vulnerabilidades pasadas.
Los requisitos de seguridad definen nuevas características o adiciones a características existentes para resolver un problema de seguridad específico o eliminar posibles vulnerabilidades.

Los requisitos de seguridad también proporcionan una base de funcionalidad de seguridad meticulosamente verificada para una aplicación.
En lugar de crear un enfoque personalizado de seguridad para cada aplicación,
los requisitos de seguridad estándar permiten a los desarrolladores reutilizar la definición de controles de seguridad y mejores prácticas;
esos mismos requisitos de seguridad cuidadosamente  verificados proporcionan soluciones para problemas de seguridad que han ocurrido en el pasado.

La importancia de comprender los requisitos clave de seguridad se describe en la práctica de [Requisitos de Seguridad][sammdsr]
que es parte de la sección de función empresarial [Diseño][sammd] dentro del [modelo SAMM][samm] de OWASP.
Idealmente, los requisitos de seguridad de software estructurados están disponibles dentro de un marco de requisitos de seguridad,
y estos son utilizados por equipos de desarrollo y equipos de producto.
Además, los proveedores de la organización deben cumplir con los requisitos de seguridad;
incorporar la seguridad en los acuerdos con proveedores para garantizar el cumplimiento de los requisitos de seguridad organizacionales.

En resumen, los requisitos de seguridad existen para prevenir la repetición de fallos de seguridad pasados.

Secciones:

3.1 [Requisitos en la práctica](#requirements-in-practice)  
3.2 [Perfil de riesgo](#risk-profile)  
3.3 [OpenCRE](#opencre)  
3.4 [SecurityRAT](#security-rat)  
3.5 [Requisitos ASVS](#asvs-requirements)  
3.6 [Requisitos MAS](#mas-requirements)  
3.7 [Requisitos SKF](#skf-requirements)  

----

La Guía de Desarrollador OWASP es un esfuerzo comunitario; si hay algo que necesite cambios, [cree un issue][issue0500].

[issue0500]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2005-requirements/00-toc
[samm]: https://owaspsamm.org/about/
[sammd]: https://owaspsamm.org/model/design/
[sammdsr]: https://owaspsamm.org/model/design/security-requirements/
