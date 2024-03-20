---

title: OWASP Secure Headers Project
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 7330
permalink: /release/implementation/secure_libraries/secure_headers/

---

{% include breadcrumb.html %}

### 5.3.3 OWASP Secure Headers Project

The OWASP Secure Headers Project ([OSHP][oshp]) provides information on HTTP response headers
to increase the security of a web application.

The OSHP documentation project is an OWASP Lab Project and intends to raise awareness and use of secure headers.

#### What is OSHP?

The [OSHP project][oshp]) provides explanations for the HTTP response headers that an application can use
to increase the security of the application.
Once set the HTTP response headers can restrict modern browsers from running into easily preventable vulnerabilities.

OSHP contains guidance and downloads on:

* Response headers explanations and usage
* Links to individual browser support
* Guidance and best practices
* Technical resources in the form of tools and documents
* Code snippets to help working with HTTP security headers

#### Why use it?

The OSHP is a documentation project that explains the reasoning and usage of HTTP response headers.
It is the go-to document for guidance and best practices;
the information on HTTP response headers is the best advice in the one location and is kept up to date.

#### How to use it

The OWASP Spotlight series provides an overview of this project and its uses:
'Project 24 - [OWASP Security Headers Project][spotlight24]'.

OSHP provides links to development [libraries][oshp-libs] that provide for secure HTTP response headers
in a range of languages and frameworks: DotNet, Go, HAPI, Java, NodeJS, PHP, Python, Ruby, Rust.
OSHP also lists [various tools][oshp-tools] useful for inspection, analysis and scanning of HTTP response headers.

----

[oshp]: https://owasp.org/www-project-secure-headers/
[oshp-libs]: https://owasp.org/www-project-secure-headers/#development-libraries
[oshp-tools]: https://owasp.org/www-project-secure-headers/#analysis-tools
[spotlight24]: https://youtu.be/N4F3VWQYU9E

\newpage
