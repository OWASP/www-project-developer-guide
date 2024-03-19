---

title: Validate All Inputs Checklist
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 625
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
and use the checklists below as suggestions for the checklist that has been tailored for the individual project.

#### Syntax and semantic validity

* Identify all data sources and classify them into trusted and untrusted
* Validate all input data from untrusted sources such as client provided data
* Encode input to a common character set before validating
* Specify character sets, such as UTF-8, for all input sources
* If the system supports UTF-8 extended character sets then validate after UTF-8 decoding is completed
* Verify that protocol header values in both requests and responses contain only ASCII characters
* Validate data from redirects
* Validate data range and also data length
* Utilize canonicalization to address obfuscation attacks
* All validation failures should result in input rejection

#### Libraries and frameworks

* Conduct all input validation on a trusted system
* Use a centralized input validation library or framework for the whole application
* If the standard validation routine cannot address some inputs then use extra discrete checks
* If any potentially hazardous input _must_ be allowed then implement additional controls
* Validate for expected data types using an allow-list rather than a deny-list

#### Validate serialized data

* Implement integrity checks or encryption of the serialized objects
    to prevent hostile object creation or data tampering
* Enforce strict type constraints during deserialization before object creation;
    typically a definable set of classes is expected
* Isolate features that deserialize so that they run in very low privilege environments such as temporary containers
* Log security deserialization exceptions and failures
* Restrict or monitor incoming and outgoing network connectivity from containers or servers that deserialize
* Monitor deserialization, for example alerting if a user agent constantly deserializes

#### References

* OWASP [Cheat Sheet: Input Validation][ivcs]
* OWASP [Java HTML Sanitizer Project][sanitizer]
* OWASP [Top 10 Proactive Controls][proactive10]

----

[control5]: https://owasp.org/www-project-proactive-controls/v3/en/c5-validate-inputs
[ivcs]: https://cheatsheetseries.owasp.org/cheatsheets/Input_Validation_Cheat_Sheet.html
[proactive10]: https://owasp.org/www-project-proactive-controls/
[sanitizer]: https://www.owasp.org/index.php/OWASP_Java_HTML_Sanitizer

\newpage
