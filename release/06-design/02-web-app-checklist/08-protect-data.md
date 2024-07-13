---

title: Protect Data Everywhere Checklist
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 6280
permalink: /release/design/web_app_checklist/protect_data/

---

{% include breadcrumb.html %}

### 4.2.8 Checklist: Protect Data Everywhere

Sensitive data such as passwords, credit card numbers, health records, personal information and business secrets
require extra protection, particularly if that data falls under privacy laws (EU General Data Protection Regulation GDPR),
financial data protection rules such as PCI Data Security Standard (PCI DSS) or other regulations.

Refer to proactive control [C8: Protect Data Everywhere][control8]
for more context from the OWASP Top 10 Proactive Controls project,
and use the list below as suggestions for a checklist that has been tailored for the individual project.

#### 1. Data protection

1. Classify data according to the level of sensitivity
1. Implement appropriate access controls for sensitive data
1. Encrypt data in transit
1. Ensure secure communication channels are properly configured
1. Avoid storing sensitive data when at all possible
1. Ensure sensitive data at rest is cryptographically protected to avoid unauthorized disclosure and modification
1. Purge sensitive data when that data is no longer required
1. Store application-level secrets in a secrets vault
1. Check that secrets are not stored in code, config files or environment variables
1. Implement least privilege, restricting access to functionality, data and system information
1. Protect all cached or temporary copies of sensitive data from unauthorized access
1. Purge those temporary copies of sensitive data as soon as they are no longer required

#### 2. Memory management

1. Explicitly initialize all variables and data stores
1. Check that any buffers are as large as specified
1. Check buffer boundaries if calling the function in a loop and protect against overflow
1. Specifically close resources, don't rely on garbage collection
1. Use non-executable stacks when available
1. Properly free allocated memory upon the completion of functions and at all exit points
1. Overwrite any sensitive information stored in allocated memory at all exit points from the function
1. Protect shared variables and resources from inappropriate concurrent access

#### References

* OWASP [Cheat Sheet: Cryptographic Storage][cscs]
* OWASP [Cheat Sheet: Secrets Management][cssm]
* OWASP [Top 10 Proactive Controls][proactive10]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue060208] or [edit on GitHub][edit060208].

[control8]: https://owasp.org/www-project-proactive-controls/v3/en/c8-protect-data-everywhere
[cscs]: https://cheatsheetseries.owasp.org/cheatsheets/Cryptographic_Storage_Cheat_Sheet.html
[cssm]: https://cheatsheetseries.owasp.org/cheatsheets/Secrets_Management_Cheat_Sheet.html
[issue060208]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/02-web-app-checklist/08-protect-data
[edit060208]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/02-web-app-checklist/08-protect-data.md
[proactive10]: https://owasp.org/www-project-proactive-controls/
