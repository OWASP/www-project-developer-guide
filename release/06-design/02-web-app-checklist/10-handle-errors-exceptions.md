---

title: Handle all Errors and Exceptions Checklist
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 6300
permalink: /release/design/web_app_checklist/handle_errors_and_exceptions/

---

{% include breadcrumb.html %}

### 4.2.10 Checklist: Handle all Errors and Exceptions

Handling exceptions and errors correctly is critical to making your code reliable and secure.
Error and exception handling occurs in all areas of an application including critical business logic
as well as security features and framework code.

Refer to proactive control [C10: Handle all Errors and Exceptions][control10]
for more context from the OWASP Top 10 Proactive Controls project,
and use the list below as suggestions for a checklist that has been tailored for the individual project.

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

[control10]: https://owasp.org/www-project-proactive-controls/v3/en/c10-errors-exceptions
[handle]: https://owasp.org/www-community/Improper_Error_Handling
[proactive10]: https://owasp.org/www-project-proactive-controls/
[review]: https://owasp.org/www-project-code-review-guide/
