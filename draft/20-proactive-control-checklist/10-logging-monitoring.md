---

title: Implement Security Logging and Monitoring Checklist
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 2010

---

{% include breadcrumb.html %}

### 20.10 Checklist: Implement Security Logging and Monitoring

Logging is recording security information during the runtime operation of an application.
Monitoring is the live review of application and security logs using various forms of automation.

Refer to proactive control '[C9: HImplement Security Logging and Monitoring][control9]'
for more context from the 'OWASP Top 10 Proactive Controls' project.

#### Security logging

* Log submitted data that is outside of an expected numeric range.
* Log submitted data that involves changes to data that should not be modifiable
* Log requests that violate server-side access control rules
* Encode and validate any dangerous characters before logging to prevent log injection attacks
* Do not log sensitive information
* Logging controls should support both success and failure of specified security events
* Do not store sensitive information in logs, including unnecessary system details, session identifiers or passwords
* Use a cryptographic hash function to validate log entry integrity

#### Security logging design

* Protect log integrity
* Ensure log entries that include untrusted data will not execute as code in the intended log viewing interface or software
* Restrict access to logs to only authorized individuals
* Utilize a central routine for all logging operations
* Forward logs from distributed systems to a central, secure logging service
* Follow a common logging format and approach within the system and across systems of an organization
* Synchronize across nodes to ensure that timestamps are consistent
* All logging controls should be implemented on a trusted system
* Ensure that a mechanism exists to conduct log analysis

#### References

* OWASP [Cheat Sheet: Logging][cslogging]
* OWASP [Cheat Sheet: Application Logging Vocabulary][csvocabulary]
* OWASP [Top 10 Proactive Controls][proactive10]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue2010] or a [pull request][pr].

[control9]: https://owasp.org/www-project-proactive-controls/v3/en/c9-security-logging.html
[cslogging]: https://cheatsheetseries.owasp.org/cheatsheets/Logging_Cheat_Sheet.html
[csvocabulary]: https://cheatsheetseries.owasp.org/cheatsheets/Logging_Vocabulary_Cheat_Sheet.html
[issue2010]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2020-proactive-control-checklist/10-logging-monitoring
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls
[proactive10]: https://owasp.org/www-project-proactive-controls/

\newpage
