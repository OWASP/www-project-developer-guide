---

title: Introduction
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 300

---

{% include breadcrumb.html %}

### 1. Introduction

Welcome to the OWASP Development Guide.

The Open Worldwide Application Security Project ([OWASP][about]) is a nonprofit foundation
that works to improve the security of software.
It is an open community dedicated to enabling organizations to
conceive, develop, acquire, operate, and maintain applications that can be trusted.

Along with the OWASP Top Ten, the Developer Guide is one of the original resources
published soon after the OWASP foundation was formed in 2001.
Version 1.0 of the Developer Guide was released in 2002
and since then there have been various [releases][versions] culminating in version 2.0 in 2005.
Since then the guide has been revised extensively to bring it up to date and no longer has version numbers;
notionally it is version 4.x as version 3.0 was never released.

The purpose of this guide is to provide an introduction to security concepts
and a handy reference for application / system developers.
Generally it describes the security practices within the Design and Implementation business functions
of the OWASP Software Assurance Maturity Model ([SAMM][samm]).
Much of this guide is based on various OWASP sources:

* [OWASP Top 10][top10]
* [Top 10 Proactive Controls][proactive10]
* [Application Security Verification Standard ((ASVS)][asvs]
* [Cheat Sheet Series][cheat]
* [Integration Standards project][wayfinder]
* [Mobile Application Security][mas]
* [Software Assurance Maturity Model (SAMM)][samm]
* [Web Security Testing Guide][wstg]

These resources provide greater detail and wider context for the various sections in this guide,
and are referenced throughout this developer guide.

The content of the main sections is aimed at an introductory level, with more detail provided in the following sections.
This guide does not seek to replicate the many excellent sources on specific security topics;
it will rarely deal with a subject at an advanced level and instead provides links for specialist security topics.

All of the OWASP projects and tools are free to download and use and the source code is open;
if you are interested in improving application security then do get involved.

#### Audience

The OWASP Developer Guide has been written by the security community to help software developers write solid,
safe and secure applications.
Application developers should try to be familiar with the entire guide;
it is far harder to write solid applications than to destroy them.

You can regard the purpose of this guide as answering the question:
 “I am a developer and I need a reference source to navigate the numerous projects
 and describe the security activities I am _supposed_ to be doing”

Or you can regard this guide as a companion document to the OWASP [Wayfinder][wayfinder] project;
the Wayfinder maps out many OWASP tools and documents, the Developer Guide provides context for them.

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue03] or a [pull request][pr] .

[about]: https://owasp.org/about/
[asvs]: https://owasp.org/www-project-application-security-verification-standard/
[cheat]: https://owasp.org/www-project-cheat-sheets/
[issue03]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2003-introduction
[mas]: https://mas.owasp.org/
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls
[proactive10]: https://owasp.org/www-project-proactive-controls/
[samm]: https://owaspsamm.org/about/
[top10]: https://owasp.org/www-project-top-ten/
[versions]: https://github.com/OWASP/DevGuide/wiki#old-versions
[wayfinder]: https://owasp.org/www-project-integration-standards/
[wstg]: https://owasp.org/www-project-web-security-testing-guide/

\newpage
