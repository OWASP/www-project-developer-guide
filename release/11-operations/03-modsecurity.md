---

title: ModSecurity Web Application Firewall
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 11030
permalink: /release/operations/modsecurity_waf/

---

{% include breadcrumb.html %}

### 9.3 ModSecurity Web Application Firewall

[ModSecurity][modsecurity] is an open source Web Application Firewall (WAF) widely deployed on web servers
that has been in continuous development and widespread use since 2002.

In 2024 it became an OWASP Production project, supported by the existing leadership and contributors.

#### What is ModSecurity?

In January 2024 the [ModSecurity][modsecurity] Web Application Firewall project was [adopted by OWASP][modsecpress],
previously [TrustWave][trustwave] had been the custodian of this project.
ModSecurity itself has a long history as an open source project, the first release was in November 2002,
and is widely used as a web application firewall for cloud and on-premises web servers.

The ModSecurity WAF needs to be configured in operational deployments,
and this can be done using the OWASP ModSecurity [Core Rule Set][modcrs].

#### Why use ModSecurity?

Web Application Firewalls are often the first line of defense against HTTP attacks on web applications and servers.
The ModSecurity WAF is widely used for this purpose along with the [Coraza WAF][coraza], also provided by OWASP.

#### How to use ModSecurity

ModSecurity is a Web Application Firewall, which scans the incoming and outgoing HTTP traffic to a web server.
The ModSecurity WAF is deployed as a proxy server in front of a web application,
or deployed within the web server itself, to provide protection against HTTP attacks.

The rules applied to the HTTP traffic are provided as configuration to ModSecurity,
and these rules allow many different actions to be applied such as blocking traffic, redirecting requests, and many more.
See the documentation for [deploying and running][modsecdocs] ModSecurity,
along with the documentation on configuring ModSecurity with the [Core Rule Set][modcrsdocs].

----

[coraza]: https://coraza.io/
[modcrs]: https://owasp.org/www-project-modsecurity-core-rule-set/
[modcrsdocs]: https://coreruleset.org/
[modsecdocs]: https://www.modsecurity.org/
[modsecurity]: https://owasp.org/www-project-modsecurity/
[modsecpress]: https://owasp.org/blog/2024/01/09/ModSecurity.html
[trustwave]: https://www.trustwave.com/
