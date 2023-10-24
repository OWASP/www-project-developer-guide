---

title: Protect Data Everywhere Checklist
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 1408

---

{% include breadcrumb.html %}

### 12.8 Checklist: Protect Data Everywhere

Sensitive data such as passwords, credit card numbers, health records, personal information and business secrets
require extra protection, particularly if that data falls under privacy laws (EU General Data Protection Regulation GDPR),
financial data protection rules such as PCI Data Security Standard (PCI DSS) or other regulations.

Refer to proactive control [C8: Protect Data Everywhere][control8]
for more context from the OWASP Top 10 Proactive Controls project,
and use the checklists below as suggestions for the checklist that has been tailored for the individual project.

#### Data protection

* Classify data according to the level of sensitivity
* Implement appropriate access controls for sensitive data
* Encrypt data in transit
* Ensure secure communication channels are properly configured
* Avoid storing sensitive data when at all possible
* Ensure sensitive data at rest is cryptographically protected to avoid unauthorized disclosure and modification
* Purge sensitive data when that data is no longer required
* Store application-level secrets in a secrets vault
* Check that secrets are not stored in code, config files or environment variables
* Implement least privilege, restricting access to functionality, data and system information
* Protect all cached or temporary copies of sensitive data from unauthorized access
* Purge those temporary copies of sensitive data as soon as they are no longer required

#### Memory management

* Explicitly initialize all variables and data stores
* Check that any buffers are as large as specified
* Check buffer boundaries if calling the function in a loop and protect against overflow
* Specifically close resources, don't rely on garbage collection
* Use non-executable stacks when available
* Properly free allocated memory upon the completion of functions and at all exit points
* Overwrite any sensitive information stored in allocated memory at all exit points from the function
* Protect shared variables and resources from inappropriate concurrent access

#### References

* OWASP [Cheat Sheet: Cryptographic Storage][cscs]
* OWASP [Cheat Sheet: Secrets Management][cssm]
* OWASP [Top 10 Proactive Controls][proactive10]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue1408] or a [pull request][pr].

[control8]: https://owasp.org/www-project-proactive-controls/v3/en/c8-protect-data-everywhere
[cscs]: https://cheatsheetseries.owasp.org/cheatsheets/Cryptographic_Storage_Cheat_Sheet.html
[cssm]: https://cheatsheetseries.owasp.org/cheatsheets/Secrets_Management_Cheat_Sheet.html
[issue1408]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2014-checklist/08-protect-data
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls
[proactive10]: https://owasp.org/www-project-proactive-controls/

\newpage
