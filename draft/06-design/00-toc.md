---

title: Design
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order:

---

{% include breadcrumb.html %}

## 4. Design

Referring to the [Secure Product Design Cheat Sheet][spdcs], the purpose of secure product design is to ensure
that all products meet or exceed the security requirements laid down by the organization.

A secure design will help establish secure defaults, minimise the attack surface area
and fail securely to well-defined and understood defaults.
It will also consider and follow various principles, such as:

* Least Privilege and Separation of Duties
* Defense-in-Depth
* Zero Trust
* Security in the Open

A Secure Development Lifecycle (SDLC) helps to ensure that all security decisions made about the product being developed
are explicit choices and result in the correct level of security for the product design.
Various secure development lifecycles can be used and they generally include threat modeling in the design process.

Sections:

4.1 [Threat modeling](#threat-modeling)  
4.1.1 [Threat modeling in practice](#threat-modeling-in-practice)  
4.1.2 [Pythonic Threat Modeling](#pythonic-threat-modeling)  
4.1.3 [Threat Dragon](#threat-dragon)  
4.1.4 [Threat Modeling and Cornucopia](#cornucopia)  
4.1.5 [Threat Modeling toolkit](#threat-modeling-toolkit)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0600] or a [pull request][pr].

[issue0600]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/00-toc
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls
[spdcs]: https://cheatsheetseries.owasp.org/cheatsheets/Secure_Product_Design_Cheat_Sheet.html

\newpage
