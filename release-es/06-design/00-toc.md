---

title: Diseño
layout: col-document
tags: Guía del Desarrollador OWASP
contributors:
document: Guía del Desarrollador OWASP
order:

---

{% include breadcrumb.html %}

![WIP logo](../../assets/images/dg_wip.png "Trabajo en curso"){height=180px}

## 4. Diseño

No hay traducción de esta página, consulte [versión original en inglés][release0600].

Sections:

4.1 [Modelado de amenazas](#modelado-de-amenazas)  
4.1.1 [Modelado de amenazas en la práctica](#modelado-de-amenazas-en-la-práctica)  
4.1.2 [pytm](#pytm)  
4.1.3 [Threat Dragon](#threat-dragon)  
4.1.4 [Cornucopia](#cornucopia)  
4.1.5 [LINDDUN GO](#linddun-go)  
4.1.6 [Kit de herramientas de modelado de amenazas](#kit-de-herramientas-de-modelado-de- amenazas)  
4.2 [Lista de verificación de aplicaciones web](#lista-de-verificación-de-aplicaciones-web)  
4.2.1 [Definir requisitos de seguridad](#definir-requisitos-de-seguridad)  
4.2.2 [Aprovechar los frameworks y librerías](#aprovechar-los-frameworks-y-librerías)  
4.2.3 [Asegurar el acceso a la base de datos](#asegurar-el-acceso-a-la-base-de-datos)  
4.2.4 [Codificar y escapar caracteres especiales en datos](#codificar-y-escapar-caracteres-especiales-en-datos)  
4.2.5 [Validar todas las entradas](#validar-todas-las-entradas)  
4.2.6 [Implementar identidad digital](#implementar-identidad-digital)  
4.2.7 [Hacer respetar los controles de acceso](#hacer-respetar-los-controles-de-acceso)  
4.2.8 [Proteger los datos en todas partes](#proteger-los-datos-en-todas-partes)  
4.2.9 [Implementar registro y monitoreo](#implementar-registro-y-monitoreo)  
4.2.10 [Manejar todos los errores y excepciones](#cmanejar-todos-los-errores-y-excepciones)  
4.3 [MAS lista de verificación](#mas-lista-de-verificación)  

----

[release0600]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/06-design/toc.md

\newpage
