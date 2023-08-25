---

title: Secure Database Access Checklist
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 2004

---

{% include breadcrumb.html %}

### 20.4 Checklist: Secure Database Access

![Developer Guide](../assets/images/dg_wip.png "OWASP Developer Guide"){: height="220px" }

The OWASP Development Guide is being rewritten by the OWASP community,
and the content has yet to be filled in for section 'C3: Secure Database Access'.

If you would like to contribute then follow the [contributing guidelines][contribute]
and submit your content for review.

[contribute]: https://github.com/OWASP/www-project-developer-guide/blob/main/contributing.md

## Database security

- [ ]   Use strongly typed parameterized queries

- [ ]   Utilize input validation and output encoding and be sure to address
    meta characters. If these fail, do not run the database command

- [ ]   Ensure that variables are strongly typed

- [ ]   The application should use the lowest possible level of privilege
    when accessing the database

- [ ]   Use secure credentials for database access

- [ ]   Connection strings should not be hard coded within the application.
    Connection strings should be stored in a separate configuration
    file on a trusted system and they should be encrypted.

- [ ]   Use stored procedures to abstract data access and allow for the
    removal of permissions to the base tables in the database

- [ ]   Close the connection as soon as possible

- [ ]   Remove or change all default database administrative passwords

- [ ]   Turn off all unnecessary database functionality

- [ ]   Remove unnecessary default vendor content (for example sample schemas)

- [ ]   Disable any default accounts that are not required to support business requirements

- [ ]   The application should connect to the database with different
    credentials for every trust distinction (for example user, read-only
    user, guest, administrators)

\newpage
