---

title: Diseño
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Roxana Calderon
document: Guía del Desarrollador OWASP
order:

---

{% include breadcrumb.html %}

![Logo de la guía del desarrollador](../../assets/images/dg_logo.png "Guía del Desarrollador OWASP"){height=180px}

## 4. Diseño

Refiriéndose a la [Hoja de Referencia de Diseño de Producto Seguro][spdcs],
el propósito de la arquitectura y diseño seguros es garantizar
que todos los productos cumplan o excedan los requisitos de seguridad establecidos por la organización,
centrándose en la seguridad vinculada a los componentes y tecnologías utilizados durante el desarrollo de la aplicación.

El Diseño de Arquitectura Segura examina la selección y composición de componentes que forman la base de la solución.
La Gestión de Tecnología examina la seguridad de las tecnologías de apoyo utilizadas durante el desarrollo,
despliegue y operaciones, como el stack de tecnología de desarrollo y sus herramientas, herramientas de despliegue,
y sistemas operativos y sus herramientas.

Un diseño seguro ayudará a establecer valores predeterminados seguros, minimizar el área de superficie de ataque
y fallar de manera segura hacia valores predeterminados bien definidos y comprendidos.
También considerará y seguirá varios principios, como:

* Privilegio Mínimo y Separación de Deberes
* Defensa en Profundidad
* Confianza Cero
* Seguridad en lo Abierto

Un Ciclo de Vida de Desarrollo Seguro (SDLC) ayuda a asegurar que todas las decisiones de seguridad tomadas
sobre el producto en desarrollo sean elecciones explícitas y resulten en el nivel correcto de seguridad
para el diseño del producto.
Se pueden utilizar varios ciclos de vida de desarrollo seguro y generalmente incluyen el modelado de amenazas
en el proceso de diseño.

Las listas de verificación y las Hojas de Referencia son herramientas importantes durante el proceso de diseño;
proporcionan una referencia fácil de conocimiento y ayudan a evitar la repetición de errores y fallos de diseño.

El [Diseño][sammd] de aplicaciones de software es una de las principales funciones de negocio descritas en
el [Modelo de Madurez de Aseguramiento de Software (SAMM)][samm], e incluye prácticas de seguridad:

* [Evaluación de Amenazas][sammdta]
* [Requisitos de Seguridad][sammdsr]
* [Arquitectura de Seguridad][sammdsa]

Secciones:

4.1 [Modelado de amenazas](#threat-modeling)  
4.1.1 [Modelado de amenazas en la práctica](#threat-modeling-in-practice)  
4.1.2 [pytm](#pytm)  
4.1.3 [Threat Dragon](#threat-dragon)  
4.1.4 [Cornucopia](#cornucopia)  
4.1.5 [LINDDUN GO](#linddun-go)  
4.1.6 [Kit de herramientas de Modelado de Amenazas](#threat-modeling-toolkit)  
4.2 [Lista de verificación de aplicaciones web](#web-application-checklist)  
4.2.1 [Definir Requisitos de Seguridad](#checklist-define-security-requirements)  
4.2.2 [Aprovechar Marcos y Bibliotecas de Seguridad](#checklist-leverage-security-frameworks-and-libraries)  
4.2.3 [Acceso Seguro a Base de Datos](#checklist-secure-database-access)  
4.2.4 [Codificar y Escapar Datos](#checklist-encode-and-escape-data)  
4.2.5 [Validar Todas las Entradas](#checklist-validate-all-inputs)  
4.2.6 [Implementar Identidad Digital](#checklist-implement-digital-identity)  
4.2.7 [Aplicar Controles de Acceso](#checklist-enforce-access-controls)  
4.2.8 [Proteger Datos en Todas Partes](#checklist-protect-data-everywhere)  
4.2.9 [Implementar Registro y Monitoreo de Seguridad](#checklist-implement-security-logging-and-monitoring)  
4.2.10 [Manejar todos los Errores y Excepciones](#checklist-handle-all-errors-and-exceptions)  
4.3 [Lista de verificación de aplicaciones móviles MAS](#mas-checklist)  

----

La Guía del Desarrollador de OWASP es un esfuerzo comunitario;
si hay algo que necesita ser cambiado, [cree un issue][issue0600].

[issue0600]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/00-toc
[samm]: https://owaspsamm.org/about/
[sammd]: https://owaspsamm.org/model/design/
[sammdsa]: https://owaspsamm.org/model/design/secure-architecture/
[sammdsr]: https://owaspsamm.org/model/design/security-requirements/
[sammdta]: https://owaspsamm.org/model/design/threat-assessment/
[spdcs]: https://cheatsheetseries.owasp.org/cheatsheets/Secure_Product_Design_Cheat_Sheet
