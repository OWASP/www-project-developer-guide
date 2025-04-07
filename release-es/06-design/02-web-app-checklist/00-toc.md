---

title: Lista de Verificación para Aplicaciones Web
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Roxana Calderon
document: Guía del Desarrollador OWASP
order:

---

{% include breadcrumb.html %}

![logo de la Guía del Desarrollador](../../../assets/images/dg_logo_bbd.png "Guía del Desarrollador OWASP"){height=180px}

### 4.2 Lista de verificación para aplicaciones web

Las listas de verificación son un recurso valioso para los equipos de desarrollo.
Proporcionan estructura para establecer buenas prácticas y procesos
y también son útiles durante las revisiones de código y actividades de diseño.

Las listas de verificación que siguen son listas generales categorizadas para seguir los controles enumerados en el
proyecto [Top 10 Controles Proactivos de OWASP][proactive10].
Estas listas de verificación proporcionan sugerencias que definitivamente deben adaptarse a
los requisitos y entorno específicos de un proyecto; no están destinadas a seguirse en su totalidad.

Probablemente el mejor punto de partida para una lista de verificación es el proporcionado
por el [Estándar de Verificación de Seguridad de Aplicaciones (ASVS)][asvs].
El ASVS puede utilizarse para proporcionar un marco para una lista de verificación inicial,
según el nivel de verificación de seguridad, y esta lista de verificación inicial
del ASVS puede ampliarse utilizando las siguientes secciones de la lista de verificación.

Secciones:

4.2.1 [Definir Requisitos de Seguridad](#checklist-define-security-requirements)  
4.2.2 [Aprovechar Marcos y Bibliotecas de Seguridad](#checklist-leverage-security-frameworks-and-libraries)  
4.2.3 [Asegurar el Acceso a la Base de Datos](#checklist-secure-database-access)  
4.2.4 [Codificar y Escapar Datos](#checklist-encode-and-escape-data)  
4.2.5 [Validar Todas las Entradas](#checklist-validate-all-inputs)  
4.2.6 [Implementar Identidad Digital](#checklist-implement-digital-identity)  
4.2.7 [Aplicar Controles de Acceso](#checklist-enforce-access-controls)  
4.2.8 [Proteger los Datos en Todas Partes](#checklist-protect-data-everywhere)  
4.2.9 [Implementar Registro y Monitoreo de Seguridad](#checklist-implement-security-logging-and-monitoring)
4.2.10 [Manejar Todos los Errores y Excepciones](#checklist-handle-all-errors-and-exceptions)  

----
Traducción de versión [original en inglés][release0602].

La Guía para Desarrolladores de OWASP es un esfuerzo comunitario;
si hay algo que necesita cambiarse, [cree un issue][issue0602].

[release0602]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/06-design/02-web-app-checklist/toc.md
[asvs]: https://owasp.org/www-project-application-security-verification-standard/
[issue0602]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/02-web-app-checklist/00-toc
[proactive10]: https://owasp.org/www-project-proactive-controls/
