---

title: Table of Contents
layout: col-document
tags: Guia do Desenvolvedor do OWASP
contributors:
document: Guia do Desenvolvedor do OWASP
order: 22000
permalink: /release-pt-br/

---

{% include breadcrumb.html %}

![Guia do Desenvolvedor logo](../assets/images/dg_logo.png "Guia do Desenvolvedor do OWASP"){: height="180px" }

### Guia do Desenvolvedor do OWASP

#### A Guide to Building Secure Web Applications and Web Services

### Release version 4.1.4

1 **[Introdução](03-introduction.md)**

2 **[Fundamentos](04-foundations/toc.md)**  
2.1 [Fundamentos de segurança](04-foundations/01-security-fundamentals.md)  
2.2 [Desenvolvimento e integração seguros](04-foundations/02-secure-development.md)  
2.3 [Princípios de segurança](04-foundations/03-security-principles.md)  
2.4 [Princípios de criptografia](04-foundations/04-crypto-principles.md)  
2.5 [OWASP Top 10](04-foundations/05-top-ten.md)  

3 **[Requisitos](05-requirements/toc.md)**  
3.1 [Requisitos na prática](05-requirements/01-requirements.md)  
3.2 [Perfil de risco](05-requirements/02-risk.md)  
3.3 [OpenCRE](05-requirements/03-opencre.md)  
3.4 [SecurityRAT](05-requirements/04-security-rat.md)  
3.5 [ASVS requisitos](05-requirements/05-asvs.md)  
3.6 [MAS requisitos)](05-requirements/06-mas.md)  
3.7 [SKF requisitos](05-requirements/07-skf.md)  

4 **[Design](06-design/toc.md)**  
4.1 [Modelagem de ameaças](06-design/01-threat-modeling/toc.md)  
4.1.1 [Modelagem de ameaças na prática](06-design/01-threat-modeling/01-threat-modeling.md)  
4.1.2 [pytm](06-design/01-threat-modeling/02-pytm.md)  
4.1.3 [Threat Dragon](06-design/01-threat-modeling/03-threat-dragon.md)  
4.1.4 [Cornucopia](06-design/01-threat-modeling/04-cornucopia.md)  
4.1.5 [LINDDUN GO](06-design/01-threat-modeling/05-linddun-go.md)  
4.1.6 [Toolkit para Modelagem de Ameaças](06-design/01-threat-modeling/06-toolkit.md)  
4.2 [Lista de verificação para aplicação web](06-design/02-web-app-checklist/toc.md)  
4.2.1 [Defina Requisitos de Segurança](06-design/02-web-app-checklist/01-define-security-requirements.md)  
4.2.2 [Utilize Frameworks e Bibliotecas de Segurança](06-design/02-web-app-checklist/02-frameworks-libraries.md)  
4.2.3 [Proteja Acesso ao Banco de Dados](06-design/02-web-app-checklist/03-secure-database-access.md)  
4.2.4 [Codifique e Escape Dados](06-design/02-web-app-checklist/04-encode-escape-data.md)  
4.2.5 [Valide todas as entradas](06-design/02-web-app-checklist/05-validate-inputs.md)  
4.2.6 [Implemente Identidade Digital](06-design/02-web-app-checklist/06-digital-identity.md)  
4.2.7 [Imponha Controles de Accesso](06-design/02-web-app-checklist/07-access-controls.md)  
4.2.8 [Proteja Dados em Todos os Lugares](06-design/02-web-app-checklist/08-protect-data.md)  
4.2.9 [Implemente Registro e Monitoramento de Segurança](06-design/02-web-app-checklist/09-logging-monitoring.md)  
4.2.10 [Trate todos os Errors e Exceções](06-design/02-web-app-checklist/10-handle-errors-exceptions.md)  
4.3 [MAS Lista de verificação](06-design/03-mas-checklist.md)  

5 **[Implementação](07-implementation/toc.md)**  
5.1 [Documentação](07-implementation/01-documentation/toc.md)  
5.1.1 [Top 10 Controles Proativos](07-implementation/01-documentation/01-proactive-controls.md)  
5.1.2 [GoSCP (Práticas de Codificação Segura em Go)](07-implementation/01-documentation/02-go-scp.md)  
5.1.3 [Série de Folha de dicas](07-implementation/01-documentation/03-cheatsheets.md)  
5.2 [Dependências](07-implementation/02-dependencies/toc.md)  
5.2.1 [Dependency-Check](07-implementation/02-dependencies/01-dependency-check.md)  
5.2.2 [Dependency-Track](07-implementation/02-dependencies/02-dependency-track.md)  
5.2.3 [CycloneDX](07-implementation/02-dependencies/03-cyclonedx.md)  
5.3 [Bibliotecas Seguras](07-implementation/03-secure-libraries/toc.md)  
5.3.1 [ESAPI](07-implementation/03-secure-libraries/01-esapi.md)  
5.3.2 [CSRFGuard](07-implementation/03-secure-libraries/02-csrf-guard.md)  
5.3.3 [OSHP](07-implementation/03-secure-libraries/03-secure-headers.md)  
5.4 [MASWE](07-implementation/03-secure-libraries/04-maswe.md)

6 **[Verificação](08-verification/toc.md)**  
6.1 [Guias](08-verification/01-guides/toc.md)  
6.1.1 [WSTG](08-verification/01-guides/01-wstg.md)  
6.1.2 [MASTG)](08-verification/01-guides/02-mastg.md)  
6.1.3 [ASVS verificação](08-verification/01-guides/03-asvs.md)  
6.2 [Ferramentas](08-verification/02-tools/toc.md)  
6.2.1 [Ferramentas DAST](08-verification/02-tools/01-dast.md)  
6.2.2 [Amass](08-verification/02-tools/02-amass.md)  
6.2.3 [OWTF](08-verification/02-tools/03-owtf.md)  
6.2.4 [Nettacker](08-verification/02-tools/04-nettacker.md)  
6.2.5 [OSHP verificação](08-verification/02-tools/05-secure-headers.md)  
6.3 [Frameworks](08-verification/03-frameworks/toc.md)  
6.3.1 [secureCodeBox](08-verification/03-frameworks/01-secure-codebox.md)  
6.4 [Gerenciamento de vulnerabilidades](08-verification/04-vulnerability-management/toc.md)  
6.4.1 [DefectDojo](08-verification/04-vulnerability-management/01-defectdojo.md)  

7 **[Treinamento e Educação](09-training-education/toc.md)**  
7.1 [Aplicações Vulneráveis](09-training-education/01-vulnerable-apps/toc.md)  
7.1.1 [Juice Shop](09-training-education/01-vulnerable-apps/01-juice-shop.md)  
7.1.2 [WebGoat](09-training-education/01-vulnerable-apps/02-webgoat.md)  
7.1.3 [PyGoat](09-training-education/01-vulnerable-apps/03-pygoat.md)  
7.1.4 [Security Shepherd](09-training-education/01-vulnerable-apps/04-security-shepherd.md)  
7.2 [Secure Coding Dojo](09-training-education/02-secure-coding-dojo.md)  
7.3 [SKF](09-training-education/03-skf.md)  
7.4 [SamuraiWTF](09-training-education/04-samurai-wtf.md)  
7.5 [Projeto OWASP Top 10](09-training-education/05-top-ten.md)  
7.6 [Mobile Top 10](09-training-education/06-mobile-top-ten.md)  
7.7 [API Top 10](09-training-education/07-api-top-ten.md)  
7.8 [WrongSecrets](09-training-education/08-wrongsecrets.md)  
7.9 [OWASP Snakes and Ladders](09-training-education/09-snakes-ladders.md)  

8 **[Construção de cultura e Amadurecimento de processos](10-culture-process/toc.md)**  
8.1 [Cultura de Segurança](10-culture-process/01-security-culture.md)  
8.2 [Campeões de Segurança](10-culture-process/02-security-champions/toc.md)  
8.2.1 [Programa de Campeões de Segurança](10-culture-process/02-security-champions/01-security-champions-program.md)  
8.2.2 [Security Champions Guide](10-culture-process/02-security-champions/02-security-champions-guide.md)  
8.2.3 [Security Champions Playbook](10-culture-process/02-security-champions/03-security-champions-playbook.md)  
8.3 [SAMM](10-culture-process/03-samm.md)  
8.4 [ASVS processos](10-culture-process/04-asvs.md)  
8.5 [MAS processos](10-culture-process/05-mas.md)  

9 **[Operações](11-operations/toc.md)**  
9.1 [Diretriz de DevSecOps](11-operations/01-devsecops.md)  
9.2 [Coraza WAF](11-operations/02-coraza.md)  
9.3 [ModSecurity WAF](11-operations/03-modsecurity.md)  
9.4 [OWASP CRS](11-operations/04-crs.md)  

10 **[Métricas](12-metrics/toc.md)**  

11 **[Security gap analysis](13-security-gap-analysis/01-guides/toc.md)**  
11.1 [Guias](13-security-gap-analysis/01-guides/toc.md)  
11.1.1 [SAMM análise](13-security-gap-analysis/01-guides/01-samm.md)  
11.1.2 [ASVS análise](13-security-gap-analysis/01-guides/02-asvs.md)  
11.1.3 [MAS análise](13-security-gap-analysis/01-guides/03-mas.md)  
11.2 [BLT](13-security-gap-analysis/02-blt.md)  

12 **[Appendices](14-appendices/toc.md)**  
12.1 [O que fazer e o que não fazer na Implementação](14-appendices/01-implementation-dos-donts/toc.md)  
12.1.1 [Segurança de containers](14-appendices/01-implementation-dos-donts/01-container-security.md)  
12.1.2 [Codificação segura](14-appendices/01-implementation-dos-donts/02-secure-coding.md)  
12.1.3 [Práticas de criptografia](14-appendices/01-implementation-dos-donts/03-cryptographic-practices.md)  
12.1.4 [Spoofing de Aplicação](14-appendices/01-implementation-dos-donts/04-application-spoofing.md)  
12.1.5 [Política de Segurança de Conteúdo (CSP)](14-appendices/01-implementation-dos-donts/05-content-security-policy.md)  
12.1.6 [Tratamento de erros e exceções](14-appendices/01-implementation-dos-donts/06-exception-error-handling.md)  
12.1.7 [Gerenciamento de arquivos](14-appendices/01-implementation-dos-donts/07-file-management.md)  
12.1.8 [Gerenciamento de memória](14-appendices/01-implementation-dos-donts/08-memory-management.md)  
12.2 [O que fazer e o que não fazer na Verificação](14-appendices/02-verification-dos-donts/toc.md)  
12.2.1 [Ambiente seguro](14-appendices/02-verification-dos-donts/01-secure-environment.md)  
12.2.2 [Hardening de sistemas](14-appendices/02-verification-dos-donts/02-system-hardening.md)  
12.2.3 [Software de Código Aberto](14-appendices/02-verification-dos-donts/03-open-source-software.md)  
