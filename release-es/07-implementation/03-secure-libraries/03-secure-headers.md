---

title: Proyecto OWASP Secure Headers
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Roxana Calderon
document: Guía del Desarrollador OWASP
order: 47330
permalink: /release-es/implementación/librerías_seguras/oshp/

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

![Logo de Secure Headers](../../../../assets/images/logos/secure_headers.png "Secure Headers de OWASP"){: .image-right }

### 5.3.3 OSHP

El Proyecto OWASP Secure Headers ([OSHP][oshp]) proporciona información sobre cabeceras de respuesta HTTP para incrementar la seguridad de una aplicación web.

El proyecto de documentación OSHP es un Proyecto de Laboratorio OWASP y crea conciencia sobre las cabeceras seguras y su uso.

#### ¿Qué es OSHP?

El [proyecto OSHP][oshp] proporciona explicaciones para las cabeceras de respuesta HTTP que una aplicación puede utilizar para aumentar la seguridad de la aplicación. Una vez establecidas, las cabeceras de respuesta HTTP pueden restringir a los navegadores modernos de ejecutar vulnerabilidades fácilmente prevenibles.

OSHP contiene guías y descargas sobre:

* Explicaciones y uso de las cabeceras de respuesta
* Enlaces al soporte individual de cada navegador
* Orientación y mejores prácticas
* Recursos técnicos en forma de herramientas y documentos
* Fragmentos de código para ayudar a trabajar con cabeceras de seguridad HTTP

#### ¿Por qué usarlo?

El OSHP es un proyecto de documentación que explica el razonamiento y uso de las cabeceras de respuesta HTTP. Es el documento de referencia para orientación y mejores prácticas; la información sobre cabeceras de respuesta HTTP es el mejor consejo, en una sola ubicación, y se mantiene actualizada.

#### Cómo usarlo

La serie OWASP Spotlight proporciona una visión general de este proyecto y sus usos: 'Proyecto 24 - [Proyecto Security Headers de OWASP][spotlight24]'.

OSHP proporciona enlaces a [bibliotecas][oshp-libs] de desarrollo que proveen cabeceras de respuesta HTTP seguras en una variedad de lenguajes y frameworks: DotNet, Go, HAPI, Java, NodeJS, PHP, Python, Ruby, Rust. El OSHP también enumera [varias herramientas][oshp-tools] útiles para la inspección, análisis y escaneo de cabeceras de respuesta HTTP.

----
Traducción de versión [original en inglés][release070303].

La Guía para Desarrolladores de OWASP es un esfuerzo comunitario; si hay algo que necesita cambiarse, [cree un issue][issue070303] o [edítelo en GitHub][edit070303].

[release070303]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/07-implementation/03-secure-libraries/03-secure-headers.md
[edit070303]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/07-implementation/03-secure-libraries/03-secure-headers.md
[issue070303]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=content&template=request.md&title=Update:%2007-implementation/03-secure-libraries/03-secure-headers
[oshp]: https://owasp.org/www-project-secure-headers/
[oshp-libs]: https://owasp.org/www-project-secure-headers/#development-libraries
[oshp-tools]: https://owasp.org/www-project-secure-headers/#analysis-tools
[spotlight24]: https://youtu.be/N4F3VWQYU9E

\newpage