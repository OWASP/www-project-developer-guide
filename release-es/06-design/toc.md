---

title: Diseño
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Roxana Calderon
document: Guía del Desarrollador OWASP
order: 46000
permalink: /release-es/diseño/

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

## 4. Diseño

Refiriéndonos a la [Hoja de Referencia de Diseño de Productos Seguros][spdcs],
el propósito de la arquitectura y diseño seguros es garantizar
que todos los productos cumplan o excedan los requisitos de seguridad establecidos por la organización,
enfocándose en la seguridad vinculada a los componentes y tecnologías utilizadas durante el desarrollo de la aplicación.

El Diseño de Arquitectura Segura examina la selección y composición de componentes que forman la base de la solución.
La Gestión de Tecnología examina la seguridad de las tecnologías de apoyo utilizadas durante el desarrollo,
despliegue y operaciones, como entornos de desarrollo y herramientas,
herramientas de despliegue, y sistemas operativos y herramientas.

Un diseño seguro ayudará a establecer configuraciones predeterminadas seguras, minimizar el área de superficie de ataque
y fallar de manera segura con configuraciones predeterminadas bien definidas y comprendidas.
También considerará y seguirá varios principios, tales como:

* Privilegio Mínimo y Separación de Funciones
* Defensa en Profundidad
* Confianza Cero
* Seguridad en Abierto

Un Ciclo de Vida de Desarrollo Seguro (SDLC) ayuda a garantizar que todas las decisiones de seguridad tomadas
sobre el producto en desarrollo sean elecciones explícitas y resulten en el nivel correcto de seguridad
para el diseño del producto.
Se pueden utilizar varios ciclos de vida de desarrollo seguro y generalmente incluyen el modelado de amenazas
en el proceso de diseño.

Las Listas de Verificación y Hojas de Referencia son una herramienta importante durante el proceso de diseño;
proporcionan una referencia fácil de conocimiento y ayudan a evitar repetir errores y fallos de diseño.

El [Diseño][sammd] de aplicaciones de software es una de las principales funciones empresariales descritas en
el [Modelo de Madurez de Aseguramiento de Software (SAMM)][samm], e incluye prácticas de seguridad:

* [Evaluación de Amenazas][sammdta]
* [Requisitos de Seguridad][sammdsr]
* [Arquitectura de Seguridad][sammdsa]

Secciones:

4.1 [Modelado de amenazas](01-threat-modeling/toc.md)  
4.1.1 [Modelado de amenazas en la práctica](01-threat-modeling/01-threat-modeling.md)  
4.1.2 [pytm](01-threat-modeling/02-pytm.md)  
4.1.3 [Threat Dragon](01-threat-modeling/03-threat-dragon.md)  
4.1.4 [Cornucopia](01-threat-modeling/04-cornucopia.md)  
4.1.5 [LINDDUN GO](01-threat-modeling/05-linddun-go.md)  
4.1.6 [Kit de herramientas de modelado de amenazas](01-threat-modeling/06-toolkit.md)  
4.2 [Lista de verificación de aplicaciones web](02-web-app-checklist/toc.md)  
4.2.1 [Definir requisitos de seguridad](02-web-app-checklist/01-define-security-requirements.md)  
4.2.2 [Aprovechar marcos de trabajo
y bibliotecas de seguridad](02-web-app-checklist/02-frameworks-libraries.md)  
4.2.3 [Acceso seguro a bases de datos](02-web-app-checklist/03-secure-database-access.md)  
4.2.4 [Codificar y escapar datos](02-web-app-checklist/04-encode-escape-data.md)  
4.2.5 [Validar todas las entradas](02-web-app-checklist/05-validate-inputs.md)  
4.2.6 [Implementar identidad digital](02-web-app-checklist/06-digital-identity.md)  
4.2.7 [Hacer cumplir controles de acceso](02-web-app-checklist/07-access-controls.md)  
4.2.8 [Proteger datos en todas partes](02-web-app-checklist/08-protect-data.md)  
4.2.9 [Implementar registro y monitoreo de seguridad](02-web-app-checklist/09-logging-monitoring.md)  
4.2.10 [Manejar todos los errores
y excepciones](02-web-app-checklist/10-handle-errors-exceptions.md)  
4.3 [Lista de verificación MAS](03-mas-checklist.md)  

----
Traducción de versión [original en inglés][release0600].

La Guía del Desarrollador OWASP es un esfuerzo comunitario; si hay algo que necesita cambiarse,
[cree un issue][issue0600] o [edítelo en GitHub][edit0600].

[release0600]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/06-design/toc.md
[edit0600]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/toc.md
[issue0600]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/00-toc
[samm]: https://owaspsamm.org/about/
[sammd]: https://owaspsamm.org/model/design/
[sammdsr]: https://owaspsamm.org/model/design/security-requirements/
[sammdsa]: https://owaspsamm.org/model/design/secure-architecture/
[sammdta]: https://owaspsamm.org/model/design/threat-assessment/
[spdcs]: https://cheatsheetseries.owasp.org/cheatsheets/Secure_Product_Design_Cheat_Sheet
