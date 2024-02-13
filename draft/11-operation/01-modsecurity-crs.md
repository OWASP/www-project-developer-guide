---

title: ModSecurity Core Rule Set
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 1101
permalink: /draft/operation/modsecurity_core_rule_set/

---

{% include breadcrumb.html %}

### 9.1 ModSecurity Core Rule Set

The OWASP ModSecurity [Core Rule Set][modcrs] (CRS) project is a set of generic attack detection rules
for use with ModSecurity compatible web application firewalls such as [OWASP Coraza][coraza].
CRS is an OWASP Flagship tool project and can be [downloaded][modcrsdownload] for either Apache or IIS/Nginx web servers.

#### What is Coraza and CRS?

To Do: go into more detail about the Coraza / ModSecurity module and the Apache web server,
so that a development team can gain an overview of how this works as a WAF.

#### What is the Core Rule Set?

To Do: go into more detail about the Coraza / ModSecurity Core Rule Set
so that a development team can determine understand its use with ModSecurity.

#### Why use it?

To Do: provide more context for ModSecurity and the CRS to allows developer to determine whether to use it in the WAF.

#### How to use it

The OWASP Spotlight series provides an overview of how to use this Core Rule Set:
'Project 3 - [Core Rule Set (CRS) - 1st Line of Defense][spotlight03]'.

To Do: give a brief outline of how CRS can provide value for the development teams.
Do not repeat the project documentation itself; ideally provide a primer and a pointer to the documentation.

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue1101] or [edit on GitHub][edit1101].

[coraza]: https://coraza.io/
[edit1101]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/11-operation/01-modsecurity-crs.md
[modcrs]: https://owasp.org/www-project-modsecurity-core-rule-set/
[modcrsdownload]: https://coreruleset.org/installation/
[issue1101]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=content&template=request.md&title=Update:%2011-operation/01-modsecurity-crs
[spotlight03]: https://youtu.be/88ZMKpiZbRI

\newpage
