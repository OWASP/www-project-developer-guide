---

title: Define Security Requirements Checklist
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 1401

---

{% include breadcrumb.html %}

### 12.1 Checklist: Define Security Requirements

A security requirement is a statement of security functionality that ensures software security is being satisfied.
Security requirements are derived from industry standards, applicable laws, and a history of past vulnerabilities.

Refer to proactive control '[C1: Define Security Requirements][control1]'
for more context from the 'OWASP Top 10 Proactive Controls' project,
and use the checklists below as suggestions for the checklist that has been tailored for the individual project.

#### System configuration

* Restrict applications, processes and service accounts to the least privileges possible
* If the application must run with elevated privileges, raise privileges as late as possible, and drop as soon as possible
* Remove all unnecessary functionality and files
* Remove test code or any functionality not intended for production, prior to deployment
* The security configuration store for the application should be available in human readable form to support auditing
* Isolate development environments from production and provide access only to authorized development and test groups
* Implement a software change control system to manage and record changes to the code both in development and production

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

#### File management

* Do not pass user supplied data directly to any dynamic include function
* Require authentication before allowing a file to be uploaded
* Limit the type of files that can be uploaded to only those types that are needed for business purposes
* Validate uploaded files are the expected type by checking file headers rather than by file extension
* Do not save files in the same web context as the application
* Prevent or restrict the uploading of any file that may be interpreted by the web server.
* Turn off execution privileges on file upload directories
* When referencing existing files, use an allow-list of allowed file names and types
* Do not pass user supplied data into a dynamic redirect
* Do not pass directory or file paths, use index values mapped to pre-defined list of paths
* Never send the absolute file path to the client
* Ensure application files and resources are read-only
* Scan user uploaded files for viruses and malware

#### References

* OWASP [Application Security Verification Standard][asvs] (ASVS)
* OWASP [Mobile Application Security][mas]
* OWASP [Top 10 Proactive Controls][proactive10]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue1401] or a [pull request][pr].

[asvs]: https://owasp.org/www-project-application-security-verification-standard/
[control1]: https://owasp.org/www-project-proactive-controls/v3/en/c1-security-requirements.html
[issue1401]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2014-checklist/01-define-security-requirements
[mas]: https://mas.owasp.org/
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls
[proactive10]: https://owasp.org/www-project-proactive-controls/

\newpage
