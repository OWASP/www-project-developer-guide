---

title: Secure Database Access Checklist
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 26230
permalink: /release-pt-br/design/web_app_checklist/secure_database_access/

---

{% include breadcrumb.html %}

### 4.2.3 Checklist: Secure Database Access

Ensure that access to all data stores is secure, including both relational databases and NoSQL databases.

Refer to proactive control [C3: Secure Database Access][control3] and its [cheatsheets][csproactive-c3]
for more context from the OWASP Top 10 Proactive Controls project,
and use the list below as suggestions for a checklist that has been tailored for the individual project.

#### 1. Secure queries

1. Use Query Parameterization to prevent untrusted input being interpreted as part of a SQL command
1. Use strongly typed parameterized queries
1. Utilize input validation and output encoding and be sure to address meta characters
1. Do not run the database command if input validation fails
1. Ensure that variables are strongly typed
1. Connection strings should not be hard coded within the application
1. Connection strings should be stored in a separate configuration file on a trusted system and they should be encrypted

#### 2. Secure configuration

1. The application should use the lowest possible level of privilege when accessing the database
1. Use stored procedures to abstract data access and allow for the removal of permissions to the base tables in the database
1. Close the database connection as soon as possible
1. Turn off all unnecessary database functionality
1. Remove unnecessary default vendor content, for example sample schemas
1. Disable any default accounts that are not required to support business requirements

#### 3. Secure authentication

1. Remove or change all default database administrative passwords
1. The application should connect to the database with different credentials for every trust distinction
    (for example user, read-only user, guest, administrators)
1. Use secure credentials for database access

#### References

* OWASP [Cheat Sheet: Query Parameterization][csquery]
* OWASP [Cheat Sheet: Database Security][csdb]
* OWASP [Top 10 Proactive Controls][proactive10]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue060203] or [edit on GitHub][edit060203].

[csproactive-c3]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c3-secure-database-access
[control3]: https://owasp.org/www-project-proactive-controls/v3/en/c3-secure-database
[csdb]: https://cheatsheetseries.owasp.org/cheatsheets/Database_Security_Cheat_Sheet
[csquery]: https://cheatsheetseries.owasp.org/cheatsheets/Query_Parameterization_Cheat_Sheet
[edit060203]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/02-web-app-checklist/03-secure-database-access.md
[issue060203]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/02-web-app-checklist/03-secure-database-access
[proactive10]: https://owasp.org/www-project-proactive-controls/
