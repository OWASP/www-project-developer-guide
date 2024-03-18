---

title: Leverage Security Frameworks and Libraries Checklist
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 622
permalink: /release/design/web_app_checklist/frameworks_libraries/

---

{% include breadcrumb.html %}

### 4.2.2 Checklist: Leverage Security Frameworks and Libraries

Secure coding libraries and software frameworks with embedded security help software developers guard against
security-related design and implementation flaws.

Refer to proactive control [C2: Leverage Security Frameworks and Libraries][control2]
for more context from the OWASP Top 10 Proactive Controls project,
and use the checklist below as suggestions for the checklist that has been tailored for the individual project.

#### Security Frameworks and Libraries

* Ensure servers, frameworks and system components are running the latest approved versions and patches
* Use libraries and frameworks from trusted sources that are actively maintained and widely used
* Review all secondary applications and third party libraries to determine business necessity
* Validate safe functionality for all secondary applications and third party libraries
* Create and maintain an inventory catalog of all third party libraries using Software Composition Analysis (SCA)
* Proactively keep all third party libraries and components up to date
* Reduce the attack surface by encapsulating the library and expose only the required behaviour into your software
* Use tested and approved managed code rather than creating new unmanaged code for common tasks
* Utilize task specific built-in APIs to conduct operating system tasks
* Do not allow the application to issue commands directly to the Operating System
* Use checksums or hashes to verify the integrity of interpreted code, libraries, executables, and configuration files
* Restrict users from generating new code or altering existing code
* Implement safe updates using encrypted channels

#### References

* OWASP [Dependency Check][dependency]
* OWASP [Top 10 Proactive Controls][proactive10]

----


[control2]: https://owasp.org/www-project-proactive-controls/v3/en/c2-leverage-security-frameworks-libraries
[dependency]: https://owasp.org/www-project-dependency-check/
[proactive10]: https://owasp.org/www-project-proactive-controls/

\newpage
