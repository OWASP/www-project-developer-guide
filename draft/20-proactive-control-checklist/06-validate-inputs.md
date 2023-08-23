---

title: Control 5 Validate All Inputs
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 2006

---

{% include breadcrumb.html %}

### 20.6 C5: Validate All Inputs

Input validation is a collection of techniques that ensure only properly formatted data
may enter a software application or system component.
Refer to proactive control '[Validate All Inputs][control5]' in the 'OWASP Top 10 Proactive Controls' project.

It is vital that input validation is performed to provide the starting point for a secure application or system.
Without input validation the software application/system will continue to be vulnerable to new and varied attacks.

#### Syntax and Semantic Validity

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

#### Validate using Libraries and Frameworks

* Conduct all input validation on a trusted system
* Use a centralized input validation library or framework for the whole application
* If the standard validation routine cannot address some inputs then use extra discrete checks
* If any potentially hazardous input _must_ be allowed then implement additional controls
* Validate for expected data types using an allow-list rather than a deny-list

#### Validate Serialized Data

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

The OWASP Developer Guide is a community effort; if you see something that needs changing
then [submit an issue][issue2006] or a [pull request][pr].

[control5]: https://owasp.org/www-project-proactive-controls/v3/en/c5-validate-inputs
[ivcs]: https://cheatsheetseries.owasp.org/cheatsheets/Input_Validation_Cheat_Sheet.html
[issue2006]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2020-proactive-control-checklist/06-validate-inputs
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls
[proactive10]: https://owasp.org/www-project-proactive-controls/v3/en/c5-validate-inputs
[sanitizer]: https://www.owasp.org/index.php/OWASP_Java_HTML_Sanitizer

\newpage
