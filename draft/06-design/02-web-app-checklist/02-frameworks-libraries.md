---

title: Leverage Security Frameworks and Libraries Checklist
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 622
permalink: /draft/design/web_app_checklist/frameworks_libraries/

---

{% include breadcrumb.html %}

### 4.2.2 Checklist: Leverage Security Frameworks and Libraries

Secure coding libraries and software frameworks with embedded security help software developers guard against
security-related design and implementation flaws.

Refer to proactive control [C2: Leverage Security Frameworks and Libraries][control2]
for more context from the OWASP Top 10 Proactive Controls project,
and use the list below as suggestions for a checklist that has been tailored for the individual project.

#### 1. Security Frameworks and Libraries

1. Ensure servers, frameworks and system components are running the latest approved versions and patches
1. Use libraries and frameworks from trusted sources that are actively maintained and widely used
1. Review all secondary applications and third party libraries to determine business necessity
1. Validate safe functionality for all secondary applications and third party libraries
1. Create and maintain an inventory catalog of all third party libraries using Software Composition Analysis (SCA)
1. Proactively keep all third party libraries and components up to date
1. Reduce the attack surface by encapsulating the library and expose only the required behaviour into your software
1. Use tested and approved managed code rather than creating new unmanaged code for common tasks
1. Utilize task specific built-in APIs to conduct operating system tasks
1. Do not allow the application to issue commands directly to the Operating System
1. Use checksums or hashes to verify the integrity of interpreted code, libraries, executables, and configuration files
1. Restrict users from generating new code or altering existing code
1. Implement safe updates using encrypted channels

#### References

* OWASP [Dependency Check][dependency]
* OWASP [Top 10 Proactive Controls][proactive10]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue060202] or [edit on GitHub][edit060202].

[control2]: https://owasp.org/www-project-proactive-controls/v3/en/c2-leverage-security-frameworks-libraries
[dependency]: https://owasp.org/www-project-dependency-check/
[issue060202]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/02-web-app-checklist/02-frameworks-libraries
[edit060202]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/02-web-app-checklist/02-frameworks-libraries.md
[proactive10]: https://owasp.org/www-project-proactive-controls/

\newpage
