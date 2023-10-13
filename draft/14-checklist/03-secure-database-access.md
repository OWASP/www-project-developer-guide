---

title: Secure Database Access Checklist
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 1403

---

{% include breadcrumb.html %}

### 14.3 Checklist: Secure Database Access

Secure access to all data stores, including both relational databases and NoSQL databases.
Refer to proactive control '[C3: Secure Database Access][control3]'
for more context from the 'OWASP Top 10 Proactive Controls' project.

#### Secure queries

* Use Query Parameterization to prevent untrusted input being interpreted as part of a SQL command
* Use strongly typed parameterized queries
* Utilize input validation and output encoding and be sure to address meta characters
* Do not run the database command if input validation fails
* Ensure that variables are strongly typed
* Connection strings should not be hard coded within the application
* Connection strings should be stored in a separate configuration file on a trusted system and they should be encrypted

#### Secure configuration

* The application should use the lowest possible level of privilege when accessing the database
* Use stored procedures to abstract data access and allow for the removal of permissions to the base tables in the database
* Close the database connection as soon as possible
* Turn off all unnecessary database functionality
* Remove unnecessary default vendor content, for example sample schemas
* Disable any default accounts that are not required to support business requirements

#### Secure authentication

* Remove or change all default database administrative passwords
* The application should connect to the database with different credentials for every trust distinction
    (for example user, read-only user, guest, administrators)
* Use secure credentials for database access

#### References

* OWASP [Cheat Sheet: Query Parameterization][query]
* OWASP [Cheat Sheet: Database Security][dbsec]
* OWASP [Top 10 Proactive Controls][proactive10]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue1403] or a [pull request][pr].

[control3]: https://owasp.org/www-project-proactive-controls/v3/en/c3-secure-database.html
[dbsec]: https://cheatsheetseries.owasp.org/cheatsheets/Database_Security_Cheat_Sheet.html
[issue1403]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2014-checklist/03-secure-database-access
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls
[proactive10]: https://owasp.org/www-project-proactive-controls/
[query]: https://cheatsheetseries.owasp.org/cheatsheets/Query_Parameterization_Cheat_Sheet.html

\newpage
