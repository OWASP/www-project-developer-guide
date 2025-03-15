title: Modelado de Amenazas
layout: col-document
tags: Guía del Desarrollador OWASP
contributors: Jon Gadsden, Roxana Calderon
document: Guía del Desarrollador OWASP
order:

---

{% include breadcrumb.html %}

![logo de la Guía del Desarrollador](../../../assets/images/dg_logo_bbd.png "Guía del Desarrollador OWASP"){height=180px}

### 4.1 Modelado de amenazas

Según la [Hoja de Referencia de Modelado de Amenazas][cstm],
el modelado de amenazas es un enfoque estructurado para identificar y priorizar amenazas potenciales a un sistema.
El proceso de modelado de amenazas incluye determinar el valor que las posibles mitigaciones tendrían
para reducir o neutralizar estas amenazas.

Evaluar las amenazas potenciales durante la fase de diseño de su proyecto puede ahorrar recursos significativos
si durante una fase posterior del proyecto se requiere refactorización para incluir mitigaciones de riesgos.
Los resultados de las actividades de modelado de amenazas generalmente incluyen:

* Documentar cómo fluyen los datos a través de un sistema para identificar dónde podría ser atacado
* Identificar tantas amenazas potenciales al sistema como sea posible
* Sugerir controles de seguridad que pueden implementarse para reducir la probabilidad o el impacto de una amenaza potencial

Secciones:

4.1.1 [Modelado de amenazas en la práctica](#threat-modeling-in-practice)  
4.1.2 [pytm](#pytm)  
4.1.3 [Threat Dragon](#threat-dragon)  
4.1.4 [Cornucopia](#cornucopia)  
4.1.5 [LINDDUN GO](#linddun-go)  
4.1.6 [Kit de herramientas de modelado de amenazas](#threat-modeling-toolkit)  

----
Traducción de versión [original en inglés][release0601].

La Guía del Desarrollador de OWASP es un esfuerzo comunitario; si hay algo que necesita cambios, [cree un issue][issue0601].

[release0601]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/06-design/01-threat-modeling/00-toc.md
[cstm]: https://cheatsheetseries.owasp.org/cheatsheets/Threat_Modeling_Cheat_Sheet
[issue0601]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/01-threat-modeling/00-toc