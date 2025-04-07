---

title: Implementación de Bibliotecas Seguras
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Roxana Calderon
document: Guía del Desarrollador OWASP
order:

---

{% include breadcrumb.html %}

![Logotipo de la guía](../../../assets/images/dg_logo_bbd.png "Guía del Desarrollador OWASP"){height=180px}

### 5.3 Bibliotecas seguras

El uso de bibliotecas seguras es parte de la gestión tecnológica que ayuda a cumplir con los requisitos de seguridad.
Las bibliotecas estándar permiten la adopción de patrones de diseño comunes y soluciones de seguridad,
y proporcionan tecnologías y marcos estandarizados que pueden utilizarse en diferentes aplicaciones.

La [Gestión Tecnológica][sammdsatm] para las aplicaciones de software es descrita por SAMM como una actividad
dentro de la práctica de seguridad [Arquitectura de Seguridad][sammdsa] de SAMM,
que a su vez es parte de la función empresarial de [Diseño][sammd].

Secciones:

5.3.1 [ESAPI](#esapi)  
5.3.2 [CSRFGuard](#csrfguard)  
5.3.3 [OSHP](#oshp)  

----
Traducción de versión [original en inglés][release0703].

La Guía para Desarrolladores de OWASP es un esfuerzo comunitario;
si hay algo que necesita cambiarse, [cree un issue][issue0703].

[release0703]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/07-implementation/03-secure-libraries/toc.md
[issue0703]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2007-implementation/03-secure-libraries/00-toc
[sammd]: https://owaspsamm.org/model/design/
[sammdsa]: https://owaspsamm.org/model/design/secure-architecture/
[sammdsatm]: https://owaspsamm.org/model/design/secure-architecture/stream-b/

\newpage
