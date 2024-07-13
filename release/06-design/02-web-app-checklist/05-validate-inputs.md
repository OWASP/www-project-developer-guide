---

title: Validate All Inputs Checklist
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 6250
permalink: /release/design/web_app_checklist/validate_inputs/

---

{% include breadcrumb.html %}

### 4.2.5 Checklist: Validate All Inputs

Input validation is a collection of techniques that ensure only properly formatted data
may enter a software application or system component.

It is vital that input validation is performed to provide the starting point for a secure application or system.
Without input validation the software application/system will continue to be vulnerable to new and varied attacks.

Refer to proactive control [C5: Validate All Inputs][control5]
for more context from the OWASP Top 10 Proactive Controls project,
and use the list below as suggestions for a checklist that has been tailored for the individual project.

#### 1. Syntax and semantic validity

1. Identify all data sources and classify them into trusted and untrusted
1. Validate all input data from untrusted sources such as client provided data
1. Encode input to a common character set before validating
1. Specify character sets, such as UTF-8, for all input sources
1. If the system supports UTF-8 extended character sets then validate after UTF-8 decoding is completed
1. Verify that protocol header values in both requests and responses contain only ASCII characters
1. Validate data from redirects
1. Validate data range and also data length
1. Utilize canonicalization to address obfuscation attacks
1. All validation failures should result in input rejection

#### 2. Libraries and frameworks

1. Conduct all input validation on a trusted system[^SCP1]
1. Use a centralized input validation library or framework for the whole application
1. If the standard validation routine cannot address some inputs then use extra discrete checks
1. If any potentially hazardous input _must_ be allowed then implement additional controls
1. Validate for expected data types using an allow-list rather than a deny-list

#### 3. Validate serialized data

1. Implement integrity checks or encryption of the serialized objects
    to prevent hostile object creation or data tampering
1. Enforce strict type constraints during deserialization before object creation;
    typically a definable set of classes is expected
1. Isolate features that deserialize so that they run in very low privilege environments such as temporary containers
1. Log security deserialization exceptions and failures
1. Restrict or monitor incoming and outgoing network connectivity from containers or servers that deserialize
1. Monitor deserialization, for example alerting if a user agent constantly deserializes

#### References

* OWASP [Cheat Sheet: Input Validation][ivcs]
* OWASP [Java HTML Sanitizer Project][sanitizer]
* OWASP [Top 10 Proactive Controls][proactive10]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue060205] or [edit on GitHub][edit060205].

[control5]: https://owasp.org/www-project-proactive-controls/v3/en/c5-validate-inputs
[ivcs]: https://cheatsheetseries.owasp.org/cheatsheets/Input_Validation_Cheat_Sheet.html
[issue060205]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/02-web-app-checklist/05-validate-inputs
[edit060205]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/02-web-app-checklist/05-validate-inputs.md
[proactive10]: https://owasp.org/www-project-proactive-controls/
[sanitizer]: https://www.owasp.org/index.php/OWASP_Java_HTML_Sanitizer
[^SCP1]: maybe this
