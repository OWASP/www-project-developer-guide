---

title: Verification Frameworks
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 8300
permalink: /release/verification/frameworks/

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

![Developer guide logo](../../../assets/images/dg_logo_bbd.png "OWASP Developer Guide"){: .image-right }

### 6.3 Verification frameworks

[Verification][sammv] is one of the business functions described by the [OWASP SAMM][samm]
and both [Security Testing][sammvst] and [Requirements-driven Testing][sammvrt] are an important part of verification.

Verification testing can benefit from using frameworks to support continuous and automated security testing.
Use of a framework can provide:

* automation of a security analysis pipeline
* flexibility to run a series of tools in a pipeline
* scalability for multiple security scanners
* control interfaces

Sections:

6.3.1 [secureCodeBox](01-secure-codebox.md)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0830] or [edit on GitHub][edit0830].

[edit0830]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/08-verification/03-frameworks/toc.md
[issue0830]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2008-verification/03-frameworks/00-toc
[samm]: https://owaspsamm.org/about/
[sammv]: https://owaspsamm.org/model/verification/
[sammvrt]: https://owaspsamm.org/model/verification/requirements-driven-testing/
[sammvst]: https://owaspsamm.org/model/verification/security-testing/
