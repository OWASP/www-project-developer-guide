---

title: Foundations
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 400
permalink: /draft/foundations/

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

## 2. Foundations

There are various foundational concepts and terminology that are commonly used in software security.
Although many of these concepts are complex to implement and are based on heavy-duty theory,
the principles are often fairly straight forward and are accessible for every software engineer.

A reasonable grasp of these foundational concepts allows development teams to understand and implement
software security for the application or system under development.
This Developer Guide can only give a brief overview of these concepts,
for in-depth knowledge refer to the many texts on security such as the [The Cyber Security Body Of Knowledge][cbok].

If changes are being introduced to the security culture of an organization
then make sure there is management buy-in and clear goals to achieve.
Without these then attempts to improve the security posture will probably fail - see the
[Security Culture][culturegoal] project for the importance of getting management,
security and development teams working together.

Sections:

2.1 [Security fundamentals](01-security-fundamentals.md)  
2.2 [Secure development and integration](02-secure-development.md)  
2.3 [Principles of security](03-security-principles.md)  
2.4 [Principles of cryptography](04-crypto-principles.md)  
2.5 [OWASP Top 10](05-top-ten.md)  

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0400] or [edit on GitHub][edit0400].

[cbok]: https://www.cybok.org/
[culturegoal]: https://owasp.org/www-project-security-culture/stable/3-Goal_Setting_and_Security_Team_Collaboration/
[edit0400]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/04-foundations/toc.md
[issue0400]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2004-foundations/00-toc
