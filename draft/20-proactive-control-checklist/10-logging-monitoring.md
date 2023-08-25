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

![Developer Guide](../assets/images/dg_wip.png "OWASP Developer Guide"){: height="220px" }

The OWASP Development Guide is being rewritten by the OWASP community,
and the content has yet to be filled in for section 'C9: Implement Security Logging and Monitoring.

If you would like to contribute then follow the [contributing guidelines][contribute]
and submit your content for review.

[contribute]: https://github.com/OWASP/www-project-developer-guide/blob/main/contributing.md


- [ ]   Do not disclose sensitive information in error responses, including
    system details, session identifiers or account information

- [ ]   Use error handlers that do not display debugging or stack trace information

- [ ]   Implement generic error messages and use custom error pages

- [ ]   The application should handle application errors and not rely on the server configuration

- [ ]   Properly free allocated memory when error conditions occur

- [ ]   Error handling logic associated with security controls should deny access by default

- [ ]   All logging controls should be implemented on a trusted system

- [ ]   Logging controls should support both success and failure of specified security events

- [ ]   Ensure logs contain important log event data

- [ ]   Ensure log entries that include un-trusted data will not execute as
    code in the intended log viewing interface or software

- [ ]   Restrict access to logs to only authorized individuals

- [ ]   Utilize a central routine for all logging operations

- [ ]   Do not store sensitive information in logs, including unnecessary
    system details, session identifiers or passwords

- [ ]   Ensure that a mechanism exists to conduct log analysis

- [ ]   Log all input validation failures

- [ ]   Log all authentication attempts, especially failures

- [ ]   Log all access control failures

- [ ]   Log all apparent tampering events, including unexpected changes to state data

- [ ]   Log attempts to connect with invalid or expired session tokens

- [ ]   Log all system exceptions

- [ ]   Log all administrative functions, including changes to the security configuration settings

- [ ]   Log all backend TLS connection failures

- [ ]   Log cryptographic module failures

- [ ]   Use a cryptographic hash function to validate log entry integrity


\newpage
