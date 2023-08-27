---

title: Protect Data Everywhere Checklist
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 2009

---

{% include breadcrumb.html %}

### 20.9 Checklist: Protect Data Everywhere

Sensitive data such as passwords, credit card numbers, health records, personal information and business secrets
require extra protection, particularly if that data falls under privacy laws (EU General Data Protection Regulation GDPR),
financial data protection rules such as PCI Data Security Standard (PCI DSS) or other regulations.

Refer to proactive control '[C8: Protect Data Everywhere][control8]'
for more context from the 'OWASP Top 10 Proactive Controls' project.

#### Data Protection

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

#### Cryptographic practices

* Use peer reviewed and open solution cryptographic modules
* All cryptographic functions used to protect secrets from the application user must be implemented on a trusted system
* Cryptographic modules must fail securely
* Ensure all random elements such as numbers, file names, UUID and strings are generated
    using the cryptographic module approved random number generator
* Cryptographic modules used by the application are compliant to FIPS 140-2 or an equivalent standard
* Establish and utilize a policy and process for how cryptographic keys will be managed
* Ensure that any secret key is protected from unauthorized access
* Store keys in a proper secrets vault as described below
* Use independent keys when multiple keys are required
* Build support for changing algorithms and keys when needed
* Build application features to handle a key rotation

#### References

* OWASP [Cheat Sheet: Cryptographic Storage][cscs]
* OWASP [Cheat Sheet: Secrets Management][cssm]
* OWASP [Top 10 Proactive Controls][proactive10]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue2009] or a [pull request][pr].

[control8]: https://owasp.org/www-project-proactive-controls/v3/en/c8-protect-data-everywhere
[cscs]: https://cheatsheetseries.owasp.org/cheatsheets/Cryptographic_Storage_Cheat_Sheet.html
[cssm]: https://cheatsheetseries.owasp.org/cheatsheets/Secrets_Management_CheatSheet.html
[issue2009]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2020-proactive-control-checklist/09-protect-data
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls
[proactive10]: https://owasp.org/www-project-proactive-controls/

\newpage
