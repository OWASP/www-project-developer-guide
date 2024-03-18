---

title: Coraza Web Application Firewall
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 1102
permalink: /release/operation/coraza_waf/

---

{% include breadcrumb.html %}

### 9.2 Coraza Web Application Firewall

The [OWASP Coraza][coraza-project] project provides a golang enterprise-grade Web Application Firewall framework
that supports the [ModSecurity][modsecurity] seclang language
and is completely compatible with the OWASP [Core Rule Set][modcrs] (CRS).
Coraza is in active development as an OWASP Production code project,
with the first stable version released in September 2021 and several releases since then.

#### What is Coraza?

The [Coraza][coraza] Web Application Firewall framework is used to enforce policies,
providing a first line of security to stop attack on web applications and servers.
Coraza  can be configured using the OWASP [Core Rule Set][modcrs] and also custom policies can be created.

Coraza can be deployed:

* as a library in an existing web server
* within an application server acting as a WAF
* as a reverse proxy
* using a docker container

#### Why use Coraza?

Web Application Firewalls are usually the first line of defense against HTTP attacks on web applications and servers.
The Coraza WAF is widely used for this purpose, especially for cloud applications,
along with the long-serving OWASP [ModSecurity][modsecurity] WAF.

#### How to use Coraza

The best way to start is to create a Coraza WAF instance and then add rules to this WAF Instance,
following the Coraza [Quick Start tutorial][coraza-tutorial].

There are multiple ways of running CRS within a WAF,
and the one chosen will depend on an individual organization's deployment:

* Coraza [SPOA connector][coraza-spoa] runs the Coraza WAF as a backing service for HAProxy
* Coraza [Caddy Module][coraza-caddy] provides Web Application Firewall capabilities for Caddy
* the Coraza [Proxy WASM][coraza-wasm] filter can be loaded directly from Envoy or used as an Istio plugin
* Coraza as a [C library][coraza-lib], used for applications written in C rather than golang

----

[coraza]: https://coraza.io/
[coraza-caddy]: https://github.com/corazawaf/coraza-caddy
[coraza-lib]: https://github.com/corazawaf/libcoraza
[coraza-project]: https://owasp.org/www-project-coraza-web-application-firewall/
[coraza-spoa]: https://coraza.io/connectors/coraza-spoa/
[coraza-tutorial]: https://coraza.io/docs/tutorials/quick-start/
[coraza-wasm]: https://github.com/corazawaf/coraza-proxy-wasm
[modcrs]: https://owasp.org/www-project-modsecurity-core-rule-set/
[modsecurity]: https://owasp.org/www-project-modsecurity/

\newpage
