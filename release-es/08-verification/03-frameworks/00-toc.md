---

title: Marcos de Verificación
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Roxana Calderon
document: Guía del Desarrollador OWASP
order:

---

{% include breadcrumb.html %}

![Developer guide logo](../../../assets/images/dg_logo_bbd.png "Guía del Desarrollador OWASP"){height=180px}

### 6.3 Marcos de verificación

La [Verificación][sammv] es una de las funciones de negocio descritas por [OWASP SAMM][samm]
y tanto las [Pruebas de Seguridad][sammvst] como las [Pruebas Basadas en Requisitos][sammvrt] son una parte importante de la verificación.

Las pruebas de verificación pueden beneficiarse del uso de frameworks para apoyar pruebas de seguridad continuas y automatizadas.
El uso de un framework puede proporcionar:

* automatización de un pipeline de análisis de seguridad
* flexibilidad para ejecutar una serie de herramientas en un pipeline
* escalabilidad para múltiples escáneres de seguridad
* interfaces de control

Secciones:

6.3.1 [secureCodeBox](#securecodebox)  

----
Traducción de versión [original en inglés][release0830].

La Guía para Desarrolladores de OWASP es un esfuerzo comunitario; si hay algo que necesita cambiarse, [cree un issue][issue0830].

[release0830]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/08-verification/03-frameworks/toc.md
[issue0830]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2008-verification/03-frameworks/00-toc
[samm]: https://owaspsamm.org/about/
[sammv]: https://owaspsamm.org/model/verification/
[sammvrt]: https://owaspsamm.org/model/verification/requirements-driven-testing/
[sammvst]: https://owaspsamm.org/model/verification/security-testing/

\newpage
