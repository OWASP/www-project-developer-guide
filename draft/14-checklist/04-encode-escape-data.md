---

title: Encode and Escape Data Checklist
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 1404

---

{% include breadcrumb.html %}

### 12.4 Checklist: Encode and Escape Data

Encoding and escaping of output data are defensive techniques meant to stop injection attacks
on a target system or application which is receiving the output data.

The target system may be another software component or it may be reflected back to the initial system,
such as operating system commands,
so encoding and escaping output data helps to provide defense in depth for the system as a whole.

Refer to proactive control '[C4: Encode and Escape Data][control4]'
for more context from the 'OWASP Top 10 Proactive Controls' project,
and use the checklists below as suggestions for the checklist that has been tailored for the individual project.

#### Character encoding and canonicalization

* Apply output encoding just before the content is passed to the target system
* Conduct all output encoding on a trusted system
* Utilize a standard, tested routine for each type of outbound encoding
* Specify character sets, such as UTF-8, for all outputs
* Apply canonicalization to convert unicode data into a standard form
* Ensure the output encoding is safe for all target systems
* In particular sanitize all output used for operating system commands

#### Contextual output encoding

Contextual output encoding of data is based on how it will be utilized by the target.
The specific methods vary depending on the way the output data is used, such as HTML entity encoding.

* Contextually encode all data returned to the client from untrusted sources
* Contextually encode all output of untrusted data to queries for SQL, XML, and LDAP

#### References

* OWASP [Cheat Sheet: Injection Prevention][ipcs]
* OWASP [Java Encoder Project][encoder]
* OWASP [Top 10 Proactive Controls][proactive10]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue1404] or a [pull request][pr].

[control4]: https://owasp.org/www-project-proactive-controls/v3/en/c4-encode-escape-data.html
[encoder]: https://www.owasp.org/index.php/OWASP_Java_Encoder_Project
[ipcs]: https://cheatsheetseries.owasp.org/cheatsheets/Injection_Prevention_Cheat_Sheet.html
[issue1404]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2014-checklist/04-encode-escape-data
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls
[proactive10]: https://owasp.org/www-project-proactive-controls/

\newpage
