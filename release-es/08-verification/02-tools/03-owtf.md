---

title: OWTF
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Roxana Calderon
document: Guía del Desarrollador OWASP
order: 48230
permalink: /release/verification/tools/owtf/

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

![Logo de OWTF](../../../../assets/images/logos/owtf.png "OWTF de OWASP"){: .image-right }

### 6.2.3 OWTF

El framework ofensivo de pruebas OWASP - Offensive Web Testing Framework ([OWTF][owtf]) es una herramienta de pruebas de penetración
que proporciona a los evaluadores de penetración un marco para organizar y ejecutar conjuntos de pruebas de seguridad.
También ayuda a alinear las pruebas de penetración con varios estándares y guías de seguridad,
permitiendo que las pruebas sean más creativas y completas.

El proyecto defensor/herramienta OWTF es un Proyecto Insignia de OWASP
y puede ser descargado desde el [área de versiones][owtfdownload] del repositorio github del proyecto.

#### ¿Qué es OWTF?

La herramienta [OWTF][owtf] es un marco de pruebas de penetración utilizado para organizar y ejecutar conjuntos de herramientas de seguridad y pruebas de penetración.
Está diseñada para ejecutarse en [Kali Linux][kali]; también puede ejecutarse en MacOS pero con algunas modificaciones de scripts y rutas.

OWTF es claramente una herramienta para evaluadores de penetración tambien llamados pentesters; existe la expectativa de que el
usuario tenga una experiencia razonable y comprensión de los entornos y herramientas de pruebas de penetración.
La [documentación][owtfdocs] sobre la instalación y ejecución de OWTF no es extensa,
y se requiere un conocimiento profundo del sistema objetivo para configurar la herramienta.

#### ¿Por qué utilizarla?

[OWTF][owtf] es fácilmente configurable y se pueden crear complementos o añadir nuevas pruebas utilizando los archivos de configuración.
Se puede instalar rápidamente en [Kali Linux][kali], una distribución de Ubuntu ampliamente utilizada por evaluadores de penetración,
y permite dirigir todo un conjunto de pruebas contra el objetivo.

#### Cómo utilizarla

La [documentación][owtfdocs] de OWTF es relativamente antigua, actualizada por última vez en 2016,
y las instrucciones de [instalación][owtfinstall] pueden necesitar adaptación para ejecutarse en MacOS o Kali.

----
Traducción de versión [original en inglés][release080203].

La Guía del Desarrollador de OWASP es un esfuerzo comunitario; si hay algo que necesita cambios,
[cree un issue][issue080203] o [edítelo en GitHub][edit080203].

[release080203]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/08-verification/02-tools/03-owtf.md
[edit080203]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/08-verification/02-tools/03-owtf.md
[issue080203]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=content&template=request.md&title=Update:%2008-verification/02-tools/03-owtf
[kali]: https://www.kali.org/
[owtfinstall]: https://owtf.readthedocs.io/en/develop/installation/methods.html
[owtfdocs]: https://owtf.readthedocs.io/
[owtfdownload]: https://github.com/owtf/owtf/releases
[owtf]: https://owasp.org/www-project-owtf/

\newpage