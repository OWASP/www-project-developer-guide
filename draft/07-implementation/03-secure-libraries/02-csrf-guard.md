---

title: CSRFGuard
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 732
permalink: /draft/implementation/secure_libraries/csrf_guard/

---

{% include breadcrumb.html %}

### 5.3.2 CSRFGuard library

OWASP [CSRFGuard][csrfguard] is a library that implements a variant of the synchronizer token pattern to mitigate
the risk of Cross-Site Request Forgery (CSRF) attacks for Java applications.

The OWASP CSRFGuard library is integrated through the use of a JavaEE Filter and exposes various automated
and manual ways to integrate per-session or pseudo-per-request tokens into HTML.
When a user interacts with this HTML, CSRF prevention tokens (i.e. cryptographically random synchronizer tokens)
are submitted with the corresponding HTTP request.

CSRFGuard is an OWASP Flagship Project and is being actively maintained by a pool of international volunteers.

#### What is CSRFGuard?

To Do: go into more detail about the CSRFGuard library so that a developer
can gain an overview of what this library can provide for them.

#### Why use it?

To Do: provide more context for the CSRFGuard library that allows developers to determine
whether to use it in their project.

#### How to use it

To Do: give a brief outline of how applying the CSRFGuard library provides increased application security.
Do not repeat the project documentation itself; ideally provide a primer and a pointer to the documentation.

----

![Developer Guide](../../assets/images/dg_wip.png "OWASP Developer Guide")

The OWASP Developer Guide is a community effort and this page needs some content to be added.
If you have suggestions then [submit an issue][issue070302] and the project team can assign it to you,
or provide new content [direct on GitHub][edit070302].

[csrfguard]: https://owasp.org/www-project-csrfguard/
[issue070302]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2007-implementation/03-secure-libraries/02-csrf-guard
[edit070302]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/07-implementation/03-secure-libraries/02-csrf-guard.md

\newpage
