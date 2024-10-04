---

title: Secure Development and Integration
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 402
permalink: /draft/foundations/secure_development/

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

### 2.2 Desarrollo e integración seguros

El desarrollo seguro se describe en el Modelo de Madurez de Garantía de Software de OWASP [(SAMM)][samm] [Diseño][sammd], [Implementación][sammi] y funciones empresariales de [Verificación][sammv].

#### Preludio

La mejor introducción al desarrollo práctico de software seguro es el artículo de OWASP [Fragmentación de seguridad de aplicaciones][sdlc]:

_O cómo me preocupaba menos y me subía a hombros de gigantes._ - Spyros Gasteratos, Elie Saad

Gran parte del material de esta sección se extrae de este proyecto OWASP de [Estándares de Integración][intstand].

#### Descripción general

Casi todo el software moderno se desarrolla de manera iterativa pasando de fase en fase,
tales como identificación de requisitos del cliente, implementación y prueba.
Estas fases se revisan de forma cíclica a lo largo de la vida útil de la aplicación.
A continuación se muestra un ciclo de vida de desarrollo de software (SDLC) teórico; en la práctica, puede haber más o menos fases.
de acuerdo a los procesos adoptados por la organización.

![SDLC Lifecycle](../../../assets/images/sdlc_diag.png "notional SDLC lifecycle"){: .image-right }

Con el creciente número y sofisticación de los exploits contra casi todas las aplicaciones o sistemas empresariales,
la mayoría de las empresas han adoptado un ciclo de vida de desarrollo de software (SDLC) seguro.
El SDLC seguro nunca debe ser un ciclo de vida separado de un ciclo de vida de desarrollo de software existente.
Siempre debe ser el mismo ciclo de vida de desarrollo que antes, pero con acciones de seguridad integradas en cada fase.
de lo contrario, es posible que los ocupados equipos de desarrollo dejen de lado las acciones de seguridad.
Tenga en cuenta que, aunque Secure SDLC podría escribirse como "SSDLC", casi siempre se escribe como "SDLC".

DevOps integra y automatiza muchas de las fases del SDLC e implementa la Integración Continua (CI)
y pipelines de entrega/implementación continua (CD) para proporcionar gran parte de la automatización del SDLC.

DevOps y pipelines se han explotado con éxito con graves consecuencias a gran escala, por lo tanto, de manera similar al SDLC, muchas de las acciones de DevOps también tienen seguridad incorporada.
Secure DevOps, o DevSecOps, incorpora prácticas de seguridad en las actividades de DevOps para protegerse contra ataques y proporcionar al SDLC pruebas de seguridad automatizadas.

Ejemplos de cómo DevSecOps es "seguridad integrada" es la provisión de
Testeo de seguridad de aplicaciones interactivas, estáticas y dinámicas (IAST, SAST y DAST)
e implementar la seguridad de la cadena de suministro, y hay muchas otras actividades de seguridad que se pueden aplicar.
Consulte la [Hoja de referencia de seguridad de CI/CD][cscicd] para conocer los últimos controles de seguridad de DevSecOps.

#### Ciclo de vida de desarrollo seguro

Refiriéndose al ciclo de desarrollo [Application Security Wayfinder][intstand] de OWASP hay cuatro fases iterativas durante el desarrollo de la aplicación: Requisitos, Diseño, Implementación y Verificación.
Las otras fases se realizan de forma menos iterativa en el ciclo de desarrollo, pero forman una parte igualmente importante.
parte del SDLC: análisis de brechas, métricas, operación y por último capacitación y creación de cultura.

Todas estas fases del SDLC deben tener actividades de seguridad integradas, en lugar de realizarse como actividades separadas. Si la seguridad está integrada en estas fases, los gastos generales serán mucho menores y la resistencia de los equipos de desarrollo disminuirá. El objetivo es que el SDLC seguro se vuelva un proceso lo más familiar posible como antes, con los equipos de desarrollo asumiendo su responsabilidad sobre las actividades de seguridad dentro de cada fase.

Existen muchas herramientas y recursos de OWASP para ayudar a incorporar seguridad en el SDLC.

* **Requisitos**: en esta fase se determinan los requisitos funcionales, no funcionales y de seguridad de la aplicación.
    Los requisitos deben revisarse periódicamente y verificar su integridad y validez.
    y vale la pena considerar varias herramientas OWASP para ayudar con esto;
  * el [Estándar de verificación de seguridad de aplicaciones (ASVS)][asvs] proporciona a los desarrolladores
      con una lista de requisitos para un desarrollo seguro,
  * el [proyecto de seguridad de aplicaciones móviles][masproject] proporciona un estándar de seguridad para aplicaciones móviles
      y [SecurityRAT][srat] ayuda a identificar un conjunto inicial de requisitos de seguridad.

* **Diseño**: es importante diseñar la seguridad en la aplicación; nunca es demasiado tarde para hacerlo, pero cuanto antes, es mejor y más fácil de hacer. OWASP proporciona dos herramientas, [Pythonic Threat Modeling][pytm]
    y [Threat Dragon][tdtm], para modelado de amenazas junto con gamificación de seguridad utilizando [Cornucopia][cornucopia].

* **Implementation**: the OWASP [Top 10 Proactive Controls][proactive10] project states that they are
    "the most important control and control categories that every architect and developer should absolutely,
    100% include in every project" and this is certainly good advice. Implementing these controls can provide
    a high degree of confidence that the application or system will be reasonably secure.
    OWASP provides two libraries that can be incorporated in web applications,
    the [Enterprise Security API (ESAPI)][esapi-project] security control library
    and [CSRFGuard][csrfguard] to mitigate the risk of [Cross-Site Request Forgery][cscsrf] (CSRF) attacks,
    that help implement these proactive controls. In addition the OWASP [Cheat Sheet Series][csproject]
    is a valuable source of information and advice on all aspects of applications security.

* **Verification**: OWASP provides a relatively large number of projects that help with testing and verification.
   This is the subject of a section in this Developer Guide, and the projects are listed at the end of this section.

* **Training**: development teams continually need security training.
   Although not part of the inner SDLC iterative loop training should still be factored into the project lifecycle.
   OWASP provides many training environments and materials - see the list at the end of this section.

* **Culture Building**: a good security culture within a business organization will help greatly in keeping
   the applications and systems secure. There are many activities that all add up to create the
   security culture, the OWASP [Security Culture][culture] project goes into more detail on these activities,
   and a good Security Champion program within the business is foundational to a good security posture.
   The OWASP [Security Champions Guide][champions] provides guidance and material to create security champions
   within the development teams - ideally every team should have a security champion that has
   a special interest in security and has received further training, enabling the team to build security in.

* **Operations**: the OWASP [DevSecOps Guideline][devsecops] explains how to best implement a secure pipeline,
    using best practices and automation tools to help 'shift-left' security issues.
    Refer to the DevSecOps Guideline for more information on any of the topics within DevSecOps
    and in particular sections on Operations.

* **Supply chain**: attacks that leverage the supply chain can be devastating
    and there have been several high profile of products being successfully exploited.
    A Software Bill of Materials (SBOM) is the first step in avoiding these attacks and
    it is well worth using the OWASP [CycloneDX][cyclone] full-stack Bill of Materials (BOM) standard
    for [risk reduction in the supply chain][cschain].
    In addition the OWASP [Dependency-Track][deptrack] project is a Continuous SBOM Analysis Platform
    which can help prevent these supply chain exploits by providing control of the SBOM.

* **Third party dependencies**: keeping track of what third party libraries are included in the application,
    and what vulnerabilities they have, is easily automated. Many public repositories such as [github][github]
    and [gitlab][gitlab] offer this service along with some commercial vendors.
    OWASP provides the [Dependency-Check][depcheck] Software Composition Analysis (SCA) tool
    to track external libraries.

* **Application security testing**: there are various types of security testing that can be automated on pull-request,
   merge or nightlies - or indeed manually but they are most powerful when automated. Commonly there is
   Static Application Security Testing (SAST), which analyses the code without running it,
   and Dynamic Application Security Testing (DAST), which applies input to the application while running it in a sandbox
   or other isolated environments.
   Interactive Application Security Testing (IAST) is designed to be run manually as well as being automated,
   and provides instant feedback on the tests as they are run.

#### Further reading from OWASP

* [Cheat Sheet Series][csproject]
* [CI/CD Security Cheat Sheet][cscicd]
* [Cornucopia][cornucopia]
* [CycloneDX][cyclone] Bill of Materials (BOM) standard
* [DevSecOps Guideline][devsecops]
* [Security Champions Guide][champions]
* [Security Culture project][culture]
* [Top 10 Proactive Controls][proactive10]

#### OWASP verification projects

* [Application Security Verification Standard][asvs] (ASVS)
* [Amass project][amass]
* [Code Pulse][pulse]
* [Defect Dojo][defectdojo]
* [Mobile Application Security][masproject] (MAS)
* [Nettacker][net]
* [Offensive Web Testing Framework][owtf] (OWTF)
* [Web Security Testing Guide][wstg] (WSTG)
* [Zed Attack Proxy][zap] (ZAP)

#### OWASP training projects

* [API Security Project][apisec] (API Top 10)
* [Juice Shop][juice]
* [Mobile Top 10][mobile10]
* [Security Shepherd][sec-shep]
* [Snakes And Ladders][snakes]
* [Top Ten Web Application security risks][top10]
* [WebGoat][webgoat]

#### OWASP resources

* [CSRFGuard library][csrfguard]
* [Dependency-Check Software Composition Analysis (SCA)][depcheck]
* [Dependency-Track Continuous SBOM Analysis Platform][deptrack]
* [Enterprise Security API][esapi-project] (ESAPI)
* [Integration Standards project Application Security Wayfinder][intstand]
* [Mobile Application Security][mas] (MAS)
* [Pythonic Threat Modeling][pytm]
* [Threat Dragon][tdtm]
* [SecurityRAT][srat] (Requirement Automation Tool)

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0402] or [edit on GitHub][edit0402].

[amass]: https://owasp.org/www-project-amass/
[apisec]: https://owasp.org/API-Security
[asvs]: https://owasp.org/www-project-application-security-verification-standard/
[champions]: https://owasp.org/www-project-security-champions-guidebook/
[cscicd]: https://cheatsheetseries.owasp.org/cheatsheets/CI_CD_Security_Cheat_Sheet
[cornucopia]: https://owasp.org/www-project-cornucopia/
[cschain]: https://cheatsheetseries.owasp.org/cheatsheets/Software_Supply_Chain_Security
[cscsrf]: https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet
[csproject]: https://owasp.org/www-project-cheat-sheets/
[csrfguard]: https://owasp.org/www-project-csrfguard/
[culture]: https://owasp.org/www-project-security-culture/
[cyclone]: https://owasp.org/www-project-cyclonedx/
[depcheck]: https://owasp.org/www-project-dependency-check/
[deptrack]: https://dependencytrack.org/
[devsecops]: https://owasp.org/www-project-devsecops-guideline/
[defectdojo]: https://www.defectdojo.org/
[edit0402]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/04-foundations/02-secure-development.md
[esapi-project]: https://owasp.org/www-project-enterprise-security-api/
[github]: https://github.com/
[gitlab]: https://about.gitlab.com/
[issue0402]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2004-foundations/02-secure-development
[juice]: https://owasp.org/www-project-juice-shop/
[mas]: https://mas.owasp.org/
[masproject]: https://owasp.org/www-project-mobile-app-security/
[mobile10]: https://owasp.org/www-project-mobile-top-10/
[net]: https://owasp.org/www-project-nettacker/
[owtf]: https://owasp.org/www-project-owtf/
[proactive10]: https://owasp.org/www-project-proactive-controls/
[pulse]: https://owasp.org/www-project-code-pulse/
[pytm]: https://owasp.org/www-project-pytm/
[samm]: https://owaspsamm.org/about/
[sammd]: https://owaspsamm.org/model/design/
[sammi]: https://owaspsamm.org/model/implementation/
[sammv]: https://owaspsamm.org/model/verification/
[sdlc]: https://owasp.org/www-project-integration-standards/writeups/owasp_in_sdlc/
[sec-shep]: https://owasp.org/www-project-security-shepherd/
[snakes]: https://owasp.org/www-project-snakes-and-ladders/
[srat]: https://owasp.org/www-project-securityrat/
[tdtm]: https://owasp.org/www-project-threat-dragon/
[top10]: https://owasp.org/Top10/
[intstand]: https://owasp.org/www-project-integration-standards/
[webgoat]: https://owasp.org/www-project-webgoat/
[wstg]: https://owasp.org/www-project-web-security-testing-guide/
[zap]: https://www.zaproxy.org/

\newpage
