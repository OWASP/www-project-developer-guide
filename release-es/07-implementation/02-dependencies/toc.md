---

title: Dependencias de Implementacion
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Roxana Calderon
document: Guía del Desarrollador OWASP
order: 47200
permalink: /release-es/implementación/dependencias/

---

{% include breadcrumb.html %}

![Logo de la guía del desarrollador](../../../assets/images/dg_logo_bbd.png "Guía del Desarrollador OWASP"){height=180px}

### 5.2 Dependencias

La gestión de dependencias de software se describe en la actividad [Dependencias de Software][sammisbsd] de SAMM,
que a su vez forma parte de la práctica de seguridad [Construcción Segura][sammisb] de SAMM
dentro de la función de negocio [Implementación][sammi].

Es importante registrar todas las dependencias utilizadas en todo el entorno de producción de la aplicación.
Esto puede lograrse mediante el Análisis de Composición de Software (SCA) para identificar las dependencias de terceros.

Una Lista de Materiales de Software (SBOM) proporciona un registro de las dependencias dentro del sistema/aplicación,
y ofrece información sobre cada dependencia para que pueda ser rastreada:

* Dónde se utiliza o referencia
* Versión utilizada
* Licencia
* Información de origen y repositorio
* Estado de soporte y mantenimiento de la dependencia

Disponer de un SBOM proporciona la capacidad de averiguar rápidamente qué aplicaciones se ven afectadas por una
[Vulnerabilidad y Exposición Común][cve] (CVE) específica, o qué CVEs están presentes en una aplicación particular.

Secciones:

5.2.1 [Dependency-Check](#dependency-check)  
5.2.2 [Dependency-Track](#dependency-track)  
5.2.3 [CycloneDX](#cyclonedx)  

----
Traducción de versión [original en inglés][release0720].

La Guía del Desarrollador de OWASP es un esfuerzo comunitario;
si hay algo que necesita cambiarse entonces [cree un issue][issue0720] o [edítelo en GitHub][edit0720].

[release0720]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/07-implementation/02-dependencies/toc.md
[cve]: https://cve.mitre.org/
[issue0720]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2007-implementation/02-dependencies/toc
[edit0720]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/07-implementation/02-dependencies/toc.md
[sammi]: https://owaspsamm.org/model/implementation/
[sammisb]: https://owaspsamm.org/model/implementation/secure-build/
[sammisbsd]: https://owaspsamm.org/model/implementation/secure-build/stream-b/

\newpage
