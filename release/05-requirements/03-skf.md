---

title: Security Knowledge Framework
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 503
permalink: /release/requirements/security_knowledge_framework/

---

{% include breadcrumb.html %}

### 3.3 Security Knowledge Framework

The [Security Knowledge Framework][skf] (SKF) is an expert system application that uses various open source projects
to support development teams and security architects in building secure applications.
The Security Knowledge Framework uses the OWASP [Application Security Verification Standard] (ASVS) with code examples
to help developers in pre-development and post-development phases and create applications that are secure by design.

Having been an OWASP flagship project for many years the SKF is now no longer within the OWASP organization;
and it will continue to be referenced in the OWASP Wayfinder and other OWASP projects
because it is a flagship project for any organization.

#### What is the Security Knowledge Framework?

The [SKF][skf] is a web application that is available from the [github repo][skfinstall].
There is [a demo version][skfdemo] of SKF that is useful for exploring the multiple benefits of the SKF.
Note that SKF is in a process of migrating to a [new repository][skfrepo] so the download link may change.

The SKF provides training and guidance for application security:

* Requirements [organizer][skfreqs]
* Learning [courses][skfdemo]:
  * Developing Secure Software (LFD121)
  * Understanding the OWASP Top 10 Security Threats (SKF100)
  * Secure Software Development: Implementation (LFD105x)
* Practice [labs][skflabs]
* Documentation on [installing and using][skfdocs] the SKF

#### Why use the SKF for requirements?

The SKF organizes security requirements into various categories that provides a good starting point for application security.

* API and Web Service
* Access Control
* Architecture Design and Threat Modeling
* Authentication
* Business Logic
* Communication
* Configuration
* Data Protection
* Error Handling and Logging
* Files and Resources
* Malicious Code
* Session Management
* Stored Cryptography
* Validation Sanitization and Encoding

#### How to use the SKF for requirements

Visit the [requirements tool website][skfreqs] and select the relevant requirements from the various categories.
Export the selection to the format of your choice (Markdown, spreadsheet CSV or plain text)
and use this as a starting point for the application security requirements.

The OWASP Spotlight series provides an overview of the SKF: 'Project 7 - [Security Knowledge Framework (SKF)][spotlight07]'.

----

[skf]: https://www.securityknowledgeframework.org/
[skfdemo]: https://secureby.design/
[skfdocs]: https://skf.readme.io/docs/introduction
[skfinstall]: https://github.com/blabla1337/skf-flask/releases
[skflabs]: https://secureby.design/labs
[skfrepo]: https://github.com/Security-Knowledge-Framework
[skfreqs]: https://starfish-app-kd3eo.ondigitalocean.app/
[spotlight07]: https://youtu.be/TFX_ZBy6lNY

\newpage
