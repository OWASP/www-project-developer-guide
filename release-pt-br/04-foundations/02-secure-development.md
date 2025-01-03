---

title: Secure Development and Integration
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 24020
permalink: /release-pt-br/foundations/secure_development/

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

### 2.2 Desenvolvimento e integração seguros

Desenvolvimento seguro é descrito nas funções de negócios de [Design][sammd], [Implementação][sammi] e [Verificação][sammv]
do Modelo de Maturidade de Software Assurance da OWASP [(SAMM)][samm].
Consulte também [Cultura de Segurança][culturewhy] para obter uma boa explicação
sobre por que é importante adicionar segurança ao ciclo de vida de desenvolvimento de software.

#### Prelúdio

A melhor introdução ao desenvolvimento prático de software seguro é o
artigo OWASP [Fragmentação de segurança de aplicações] [sdlc]:

_Ou como me preocupei menos e fiquei sobre ombros de gigantes._ - Spyros Gasteratos, Elie Saad

Grande parte do material nesta seção foi extraído do projeto [Integration Standards][intstand] da OWASP.

#### Visão geral

Quase todo software moderno é desenvolvido de maneira iterativa, passando de fase em fase,
como identificação de requisitos do cliente, implementação e teste.
Estas fases são revisitadas de forma cíclica ao longo do desenvolvimento da aplicação.
Um ciclo de desenvolvimento de software (SDLC) nocional é mostrado abaixo; na prática, pode haver mais ou menos fases
de acordo com os processos adotados pela organização.

![SDLC Lifecycle](../../../assets/images/sdlc_diag.png "notional SDLC lifecycle"){: .image-right }

Com o crescente número e sofisticação de explorações contra quase todas as aplicações ou sistemas de negócios,
a maioria das empresas adotou um Ciclo de Desenvolvimento de Software (SDLC) seguro.
O SDLC seguro nunca deve ser um ciclo separado do ciclo de desenvolvimento de software preexistente,
ele deve ser sempre o mesmo ciclo de desenvolvimento de antes, mas com ações de segurança integradas em cada fase,
caso contrário, as ações de segurança poderão ser deixadas de lado por equipes de desenvolvimento atarefadas.
Observe que embora o SDLC Seguro possa ser escrito como 'SSDLC', quase sempre é escrito como 'SDLC'.

DevOps integra e automatiza muitas das fases do SDLC e implementa Integração Contínua (CI)
e pipelines de entrega/implementação contínua (CD) para fornecer grande parte da automação do SDLC.

DevOps e pipelines tem sido explorados com sucesso, com sérias consequências em grande escala
e assim, de maneira semelhante ao SDLC, muitas das ações de DevOps também tiveram segurança incorporada.
DevOps Seguro, ou DevSecOps, incorpora práticas de segurança nas atividades de DevOps para proteção contra ataques
e para fornecer testes de segurança automatizados ao SDLC.

Exemplos de como o DevSecOps é 'segurança embutida' são o fornecimento de
Testes Interativos, Estáticos e Dinâmicos (IAST, SAST e DAST) de segurança de aplicações
e a implementação de segurança da cadeia de suprimento de software, e há muitas outras atividades de segurança que podem ser aplicadas.
Consulte a [folha de dicas de segurança para CI/CD][cscicd] para obter os controles de segurança DevSecOps mais recentes.

#### Secure development lifecycle

Referring to the OWASP [Application Security Wayfinder][intstand] development cycle
there are four iterative phases during application development: Requirements, Design, Implementation and Verification.
The other phases are done less iteratively in the development cycle but these form an equally important
part of the SDLC: Gap Analysis, Metrics, Operation and Training & Culture Building.

All of these phases of the SDLC should have security activities built into them,
rather than done as separate activities. If security is built into these phases then the overhead becomes much less
and the resistance from the development teams decreases. The goal is for the secure SDLC to become as familiar
a process as before, with the development teams taking ownership of the security activities within each phase.

There are many OWASP tools and resources to help build security into the SDLC.

* **Requirements**: this phase determines the functional, non-functional and security requirements for the application.
    Requirements should be revisited periodically and checked for completeness and validity,
    and it is worth considering various OWASP tools to help with this;
  * the [Application Security Verification Standard (ASVS)][asvs] provides developers
      with a list of requirements for secure development,
  * the [Mobile Application Security project][masproject] provides a security standard for mobile applications
      and [SecurityRAT][srat] helps identify an initial set of security requirements.

* **Design**: it is important to design security into the application - it is never too late to do this
    but the earlier the better and easier to do. OWASP provides two tools, [Pythonic Threat Modeling][pytm]
    and [Threat Dragon][tdtm], for threat modeling along with security gamification using [Cornucopia][cornucopia].

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

O Guia do Desenvolvedor da OWASP é um trabalho da comunidade; se há algo que precisa ser mudado
então [submeta uma issue][issue0402] ou [edite no GitHub][edit0402].

[amass]: https://owasp.org/www-project-amass/
[apisec]: https://owasp.org/API-Security
[asvs]: https://owasp.org/www-project-application-security-verification-standard/
[champions]: https://owasp.org/www-project-security-champions-guidebook/
[cscicd]: https://cheatsheetseries.owasp.org/cheatsheets/CI_CD_Security_Cheat_Sheet
[cornucopia]: https://owasp.org/www-project-cornucopia/
[cschain]: https://cheatsheetseries.owasp.org/cheatsheets/Software_Supply_Chain_Security_Cheat_Sheet
[cscsrf]: https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet
[csproject]: https://owasp.org/www-project-cheat-sheets/
[csrfguard]: https://owasp.org/www-project-csrfguard/
[culture]: https://owasp.org/www-project-security-culture/
[culturewhy]: https://owasp.org/www-project-security-culture/stable/2-Why_Add_Security_In_Development_Teams/
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
