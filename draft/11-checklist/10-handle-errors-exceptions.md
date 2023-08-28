---

title: Handle all Errors and Exceptions Checklist
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 2011

---

{% include breadcrumb.html %}

### 20.11 Checklist: Handle all Errors and Exceptions

Handling exceptions and errors correctly is critical to making your code reliable and secure.
Error and exception handling occurs in all areas of an application including critical business logic
as well as security features and framework code.

Refer to proactive control '[C10: Handle all Errors and Exceptions][control10]'
for more context from the 'OWASP Top 10 Proactive Controls' project.

#### Errors and exceptions

* Manage exceptions in a centralized manner to avoid duplicated try/catch blocks in the code
* Ensure that all unexpected behavior is correctly handled inside the application
* Ensure that error messages displayed to users do not leak critical data,
    but are still verbose enough to enable the proper user response
* Ensure that exceptions logs give enough information for support, QA, forensics or incident response teams
* Carefully test and verify error handling code
* Do not disclose sensitive information in error responses, for example
    system details, session identifiers or account information
* Use error handlers that do not display debugging or stack trace information
* Implement generic error messages and use custom error pages
* The application should handle application errors and not rely on the server configuration
* Properly free allocated memory when error conditions occur
* Error handling logic associated with security controls should deny access by default

#### References

* OWASP [Code Review Guide: Error Handling][review]
* OWASP [Improper Error Handling][handle]
* OWASP [Top 10 Proactive Controls][proactive10]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue2010] or a [pull request][pr].

[control10]: https://owasp.org/www-project-proactive-controls/v3/en/c10-errors-exceptions.html
[handle]: https://owasp.org/www-community/Improper_Error_Handling
[issue2010]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2011-checklist/10-handle-errors-exceptions
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls
[proactive10]: https://owasp.org/www-project-proactive-controls/
[review]: https://owasp.org/www-project-code-review-guide/

\newpage
