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

OWASP Coraza is a golang enterprise-grade Web Application Firewall framework
that supports the seclang language by ModSecurity and is 100% compatible with the OWASP Core Ruleset.
Coraza is an OWASP Production project and is in active development.

#### What is Coraza?

To Do: go into more detail about Coraza Web Application Firewall framework,
so that a development team can gain an overview of how to use this as a WAF.

#### Why use it?

To Do: provide more context for Coraza to allows developer to determine whether to use it.

#### How to use it

To Do: give a brief outline of how Coraza can provide value for the development teams.
Do not repeat the project documentation itself; ideally provide a primer and a pointer to the documentation.

For example, Coraza can be imported as a library or used with one of the Coraza connectors like
[coraza-server][coraza-server] (GRPC and SPOA),
[coraza-caddy][caddy] (web server, reverse proxy) and [docker][coraza-docker] (using connector).

----

![Developer Guide](../assets/images/dg_wip.png "OWASP Developer Guide")

The OWASP Developer Guide is a community effort and this page needs some content to be added.
If you have suggestions then [submit an issue][issue1102] and the project team can assign it to you,
or provide new content [direct on GitHub][edit1102].

[caddy]: https://github.com/corazawaf/coraza-caddy
[coraza-docker]: https://owasp.org/www-project-coraza-web-application-firewall/#
[coraza-server]: https://github.com/corazawaf/coraza-server
[issue1102]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2011-operation/02-coraza
[edit1102]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/11-operation/02-coraza.md

\newpage
