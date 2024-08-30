---

title: Introduction
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 3000
permalink: /release-pt-br/introduction/

---

{% include breadcrumb.html %}

<style type="text/css">
.image-right {
  height: 180px;
  display: block;
  margin-left: auto;
  margin-right: auto;
  float: right;
}
</style>

![Developer guide logo](../../assets/images/dg_logo.png "OWASP Developer Guide"){: .image-right }

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
Since then the guide has been revised extensively to bring it up to date.
The latest versions are 4.x because version 3.0 was never released.

The purpose of this guide is to provide an introduction to security concepts
and a handy reference for application / system developers.
Generally it describes security practices using the advice given in the
OWASP Software Assurance Maturity Model ([SAMM][samm]) and describes the OWASP projects
referenced in the OWASP [Application Wayfinder][wayfinder] project.

This guide does not seek to replicate the many excellent sources on specific security topics;
it will rarely tries to go into details on a subject and instead provides links for greater depth on these security topics.
Instead the content of the Developer Guide aims to be accessible, introducing  practical security concepts
and providing enough detail to get developers started on various OWASP tools and documents.

All of the OWASP projects and tools described in this guide are free to download and use.
All OWASP projects are open source; do get involved if you are interested in improving application security.

#### Audience

The OWASP Developer Guide has been written by the security community to help software developers write solid,
safe and secure applications.
Developers should try and be familiar with most of this guide; it will help to write applications that are more secure.

You can think of this guide as a cross-reference source to the many tools and documents that OWASP provide for developers.

Or you can regard the purpose of this guide as answering the question:
 “I am a developer and I need a reference guide to navigate the numerous security tools
 and security activities that I know I should be doing.

Or think of it as a collection of articles that introduce developers to the wide domain of application security.

Or you can regard this guide as a companion document to the OWASP [Application Wayfinder][wayfinder] project:
the Wayfinder mapping out the many OWASP tools, projects and documents with the Developer Guide providing some context.

[![Application Wayfinder Diagram](../assets/images/owasp-wayfinder.png "OWASP Application Wayfinder")][wayfinder]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue03] or [edit on GitHub][edit03].

[about]: https://owasp.org/about/
[edit03]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/03-introduction.md
[issue03]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2003-introduction
[samm]: https://owaspsamm.org/about/
[versions]: https://github.com/OWASP/DevGuide/wiki#old-versions
[wayfinder]: https://owasp.org/www-project-integration-standards/
