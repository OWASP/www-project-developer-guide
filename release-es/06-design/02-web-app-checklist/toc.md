---

title: Lista de verificación de aplicaciones web
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Roxana Calderon
document: Guía del Desarrollador OWASP
order: 46200
permalink: /release-es/diseño/lista_verificación_web/

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

![Logo de la guía del desarrollador](../../../assets/images/dg_logo_bbd.png "Guía del Desarrollador OWASP"){: .image-right }

### 4.2 Lista de verificación para aplicaciones web

Las listas de verificación son un recurso valioso para los equipos de desarrollo.
Proporcionan estructura para establecer buenas prácticas y procesos,
y también son útiles durante las revisiones de código y actividades de diseño.

Las listas de verificación que siguen son listas generales categorizadas para seguir los controles enumerados en el
proyecto [Top 10 Controles Proactivos de OWASP][proactive10].
Estas listas de verificación proporcionan sugerencias que ciertamente deben adaptarse a
los requisitos y el entorno específicos de un proyecto; no están destinadas a seguirse en su totalidad.

Probablemente el mejor punto de partida para una lista de verificación es el proporcionado
por el [Estándar de Verificación de Seguridad de Aplicaciones (ASVS)][asvs].
El ASVS puede utilizarse para proporcionar un marco para una lista de verificación inicial,
según el nivel de verificación de seguridad,
y esta lista de verificación inicial del ASVS puede ampliarse utilizando las siguientes secciones de la lista.

Secciones:

4.2.1 [Definir requisitos de seguridad](01-define-security-requirements.md)  
4.2.2 [Aprovechar marcos y bibliotecas de seguridad](02-frameworks-libraries.md)  
4.2.3 [Acceso seguro a la base de datos](03-secure-database-access.md)  
4.2.4 [Codificar y escapar datos](04-encode-escape-data.md)  
4.2.5 [Validar todas las entradas](05-validate-inputs.md)  
4.2.6 [Implementar identidad digital](06-digital-identity.md)  
4.2.7 [Aplicar controles de acceso](07-access-controls.md)  
4.2.8 [Proteger datos en todas partes](08-protect-data.md)  
4.2.9 [Implementar registro y monitoreo de seguridad](09-logging-monitoring.md)  
4.2.10 [Manejar todos los errores y excepciones](10-handle-errors-exceptions.md)  

----
Traducción de versión [original en inglés][release0602].

La Guía para Desarrolladores de OWASP es un esfuerzo comunitario; si hay algo que necesita cambios,
[cree un issue][issue0602] o [edítelo en GitHub][edit0602].

[release0602]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/06-design/02-web-app-checklist/toc.md
[asvs]: https://owasp.org/www-project-application-security-verification-standard/
[edit0602]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/02-web-app-checklist/toc.md
[issue0602]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/02-web-app-checklist/00-toc
[proactive10]: https://owasp.org/www-project-proactive-controls/

/newpage
