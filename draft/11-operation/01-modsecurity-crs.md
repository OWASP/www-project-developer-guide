---

title: ModSecurity Core Rule Set
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 1101
permalink: /draft/operation/modsecurity_core_rule_set/

---

{% include breadcrumb.html %}

### 9.1 ModSecurity Core Rule Set

The OWASP ModSecurity [Core Rule Set][modcrs-project] (CRS) project is a set of generic attack detection rules
for use with [ModSecurity][modsecurity] compatible web application firewalls such as [OWASP Coraza][coraza].
CRS is an OWASP Flagship tool project and can be [downloaded][modcrs-download] for either Apache or IIS/Nginx web servers.

#### What is the Core Rule Set?

The [Core Rule Set][modcrs] (CRS) are attack detection rules for use with [ModSecurity][modsecurity],
[Coraza[coraza] and other ModSecurity compatible web application firewalls.
The CRS aims to protect web applications from a wide range of attacks with a minimum of false alerts.
The CRS provides protection against many common attack categories, including those in the OWASP Top Ten.

#### Why use it?

If an organization is using a Coraza, ModSecurity or compatible Web Application Firewall (WAF)
then it is very likely that the [Core Rule Set][modcrs] is already in use by this WAF.
The CRS provides the policy for the Coraza / Modsecurity engine so that traffic to a web application is inspected
for various attacks and malicious traffic is blocked.

#### How to use it

The use of the Core Rule Set assumes that a ModSecurity, Coraza or compatible WAF has been installed.
Refer to the [Coraza tutorial][coraza-tutorial] or the [ModSecurity][modsecdocs] on how to do this.

To get started with CRS refer to the Core Rule Set [installation instructions][modcrs-download].

The OWASP Spotlight series provides an overview of how to use this Core Rule Set:
'Project 3 - [Core Rule Set (CRS) - 1st Line of Defense][spotlight03]'.

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue1101] or [edit on GitHub][edit1101].

[coraza]: https://coraza.io/
[coraza-tutorial]: https://coraza.io/docs/tutorials/quick-start/
[edit1101]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/11-operation/01-modsecurity-crs.md
[issue1101]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=content&template=request.md&title=Update:%2011-operation/01-modsecurity-crs
[modcrs-project]: https://owasp.org/www-project-modsecurity-core-rule-set/
[modcrs-download]: https://coreruleset.org/docs/deployment/install/
[modcrs]: https://coreruleset.org/
[modsecurity]: https://owasp.org/www-project-modsecurity/
[modsecdocs]: https://www.modsecurity.org/
[spotlight03]: https://youtu.be/88ZMKpiZbRI

\newpage
