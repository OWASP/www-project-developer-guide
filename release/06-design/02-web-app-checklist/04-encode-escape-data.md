---

title: Encode and Escape Data Checklist
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 6240
permalink: /release/design/web_app_checklist/encode_escape_data/

---

{% include breadcrumb.html %}

### 4.2.4 Checklist: Encode and Escape Data

Encoding and escaping of output data are defensive techniques meant to stop injection attacks
on a target system or application which is receiving the output data.

The target system may be another software component or it may be reflected back to the initial system,
such as operating system commands,
so encoding and escaping output data helps to provide defense in depth for the system as a whole.

Refer to proactive control [C4: Encode and Escape Data][control4] and its [cheatsheets][csproactive-c4]
for more context from the OWASP Top 10 Proactive Controls project,
and use the list below as suggestions for a checklist that has been tailored for the individual project.

#### 1. Character encoding and canonicalization

1. Apply output encoding just before the content is passed to the target system
1. Conduct all output encoding on a trusted system
1. Utilize a standard, tested routine for each type of outbound encoding
1. Specify character sets, such as UTF-8, for all outputs
1. Apply canonicalization to convert unicode data into a standard form
1. Ensure the output encoding is safe for all target systems
1. In particular sanitize all output used for operating system commands

#### 2. Contextual output encoding

Contextual output encoding of data is based on how it will be utilized by the target.
The specific methods vary depending on the way the output data is used, such as HTML entity encoding.

1. Contextually encode all data returned to the client from untrusted sources
1. Contextually encode all output of untrusted data to queries for SQL, XML, and LDAP

#### References

* OWASP [Cheat Sheet: Injection Prevention][ipcs]
* OWASP [Java Encoder Project][encoder]
* OWASP [Top 10 Proactive Controls][proactive10]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue060204] or [edit on GitHub][edit060204].

[csproactive-c4]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c4-encode-and-escape-data
[control4]: https://owasp.org/www-project-proactive-controls/v3/en/c4-encode-escape-data
[edit060204]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/02-web-app-checklist/04-encode-escape-data.md
[encoder]: https://www.owasp.org/index.php/OWASP_Java_Encoder_Project
[ipcs]: https://cheatsheetseries.owasp.org/cheatsheets/Injection_Prevention_Cheat_Sheet
[issue060204]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/02-web-app-checklist/04-encode-escape-data
[proactive10]: https://owasp.org/www-project-proactive-controls/
