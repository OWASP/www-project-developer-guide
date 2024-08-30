---

title: Define Security Requirements Checklist
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 6210
permalink: /release-pt-br/design/web_app_checklist/define_security_requirements/

---

{% include breadcrumb.html %}

### 4.2.1 Checklist: Define Security Requirements

A security requirement is a statement of security functionality that ensures software security is being satisfied.
Security requirements are derived from industry standards, applicable laws, and a history of past vulnerabilities.

Refer to proactive control [C1: Define Security Requirements][control1] and its [cheatsheets][csproactive-c1]
for more context from the OWASP Top 10 Proactive Controls project,
and use the lists below as suggestions for a checklist that has been tailored for the individual project.

#### 1. System configuration

1. Restrict applications, processes and service accounts to the least privileges possible
1. If the application must run with elevated privileges, raise privileges as late as possible, and drop as soon as possible
1. Remove all unnecessary functionality and files
1. Remove test code or any functionality not intended for production, prior to deployment
1. The security configuration store for the application should be available in human readable form to support auditing
1. Isolate development environments from production and provide access only to authorized development and test groups
1. Implement a software change control system to manage and record changes to the code both in development and production

#### 2. Cryptographic practices

1. Use peer reviewed and open solution cryptographic modules
1. All cryptographic functions used to protect secrets from the application user must be implemented on a trusted system
1. Cryptographic modules must fail securely
1. Ensure all random elements such as numbers, file names, UUID and strings are generated
    using the cryptographic module approved random number generator
1. Cryptographic modules used by the application are compliant to FIPS 140-2 or an equivalent standard
1. Establish and utilize a policy and process for how cryptographic keys will be managed
1. Ensure that any secret key is protected from unauthorized access
1. Store keys in a proper secrets vault as described below
1. Use independent keys when multiple keys are required
1. Build support for changing algorithms and keys when needed
1. Build application features to handle a key rotation

#### 3. File management

1. Do not pass user supplied data directly to any dynamic include function
1. Require authentication before allowing a file to be uploaded
1. Limit the type of files that can be uploaded to only those types that are needed for business purposes
1. Validate uploaded files are the expected type by checking file headers rather than by file extension
1. Do not save files in the same web context as the application
1. Prevent or restrict the uploading of any file that may be interpreted by the web server.
1. Turn off execution privileges on file upload directories
1. When referencing existing files, use an allow-list of allowed file names and types
1. Do not pass user supplied data into a dynamic redirect
1. Do not pass directory or file paths, use index values mapped to pre-defined list of paths
1. Never send the absolute file path to the client
1. Ensure application files and resources are read-only
1. Scan user uploaded files for viruses and malware

#### References

* OWASP [Application Security Verification Standard][asvs] (ASVS)
* OWASP [Mobile Application Security][mas]
* OWASP [Top 10 Proactive Controls][proactive10]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue060201] or [edit on GitHub][edit060201].

[asvs]: https://owasp.org/www-project-application-security-verification-standard/
[csproactive-c1]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c1-define-security-requirements
[control1]: https://owasp.org/www-project-proactive-controls/v3/en/c1-security-requirements
[edit060201]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/02-web-app-checklist/01-define-security-requirements.md
[issue060201]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/02-web-app-checklist/01-define-security-requirements
[mas]: https://mas.owasp.org/
[proactive10]: https://owasp.org/www-project-proactive-controls/
