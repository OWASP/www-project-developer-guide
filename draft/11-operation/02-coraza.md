---

title: Coraza Web Application Firewall
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 1102
permalink: /draft/operation/coraza_waf/

---

{% include breadcrumb.html %}

### 9.2 Coraza Web Application Firewall

[OWASP Coraza][coraza] is a golang enterprise-grade Web Application Firewall framework
that supports the seclang language by ModSecurity and is 100% compatible with the OWASP [Core Rule Set][modcrs].
Coraza is an OWASP Production code project and is in active development.

#### What is Coraza?

To Do: go into more detail about Coraza Web Application Firewall framework,
so that a development team can gain an overview of how to use this as a WAF.

#### Why use Coraza?

To Do: provide more context for Coraza to allows developer to determine whether to use it.

#### How to use Coraza

To Do: give a brief outline of how Coraza can provide value for the development teams.
Do not repeat the project documentation itself; ideally provide a primer and a pointer to the documentation.

For example, Coraza can be imported as a library or used with one of the Coraza connectors
[coraza-server][coraza-server] (GRPC and SPOA),
[coraza-caddy][coraza-caddy] (web server, reverse proxy) and [docker][coraza-docker] (using connector).

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue1102] or [edit on GitHub][edit1102].

[coraza]: https://coraza.io/
[coraza-caddy]: https://github.com/corazawaf/coraza-caddy
[coraza-docker]: https://owasp.org/www-project-coraza-web-application-firewall/#
[coraza-server]: https://github.com/corazawaf/coraza-server
[edit1102]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/11-operation/02-coraza.md
[issue1102]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=content&template=request.md&title=Update:%2011-operation/02-coraza
[modcrs]: https://owasp.org/www-project-modsecurity-core-rule-set/

\newpage
