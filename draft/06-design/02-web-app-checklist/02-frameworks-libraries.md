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
and its [cheatsheets][csproactive-c2] for more context from the OWASP Top 10 Proactive Controls project.

For technology specific checklists refer to the appropriate OWASP Cheat Sheets:

* [AJAX_Security][csajax]
* [C-Based toolchain hardening][cscbased]
* [Django security][csdjango]
* [Django REST framework][csdjangorest]
* [Docker security][csdocker]
* [DotNet security][csdotnet]
* [GraphQL security][csgraphql]
* [Java security][csjava]
* [Javascript management][csjcavascript]
* [Kubernetes][cskube]
* [Laravel security][cslaravel]
* [Microservices security][csmicro]
* [NPM security best practices][csnpm]
* [Node.js security][csnode]
* [Node.js security for Docker][csnodedocker]
* [PHP configuration][csphp]
* [REST APIs][csrest]
* [Ruby on Rails security][csruby]
* [Symfony framework][cssymfony]
* [Web Services][cswebservice]
* [XML security][csxml]

and use them as the starting point for a checklist that is tailored for the technology used by the project.

In addition consider the following extra checks for frameworks and libraries.

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

[csajax]: https://cheatsheetseries.owasp.org/cheatsheets/AJAX_Security_Cheat_Sheet
[cscbased]: https://cheatsheetseries.owasp.org/cheatsheets/C-Based_Toolchain_Hardening_Cheat_Sheet
[csdjango]: https://cheatsheetseries.owasp.org/cheatsheets/Django_Security_Cheat_Sheet
[csdjangorest]: https://cheatsheetseries.owasp.org/cheatsheets/Django_REST_Framework_Cheat_Sheet
[csdocker]: https://cheatsheetseries.owasp.org/cheatsheets/Docker_Security_Cheat_Sheet
[csdotnet]: https://cheatsheetseries.owasp.org/cheatsheets/DotNet_Security_Cheat_Sheet
[csgraphql]: https://cheatsheetseries.owasp.org/cheatsheets/GraphQL_Cheat_Sheet
[csjava]: https://cheatsheetseries.owasp.org/cheatsheets/Java_Security_Cheat_Sheet
[csjcavascript]: https://cheatsheetseries.owasp.org/cheatsheets/Third_Party_Javascript_Management_Cheat_Sheet
[cskube]: https://cheatsheetseries.owasp.org/cheatsheets/Kubernetes_Security_Cheat_Sheet
[cslaravel]: https://cheatsheetseries.owasp.org/cheatsheets/Laravel_Cheat_Sheet
[csmicro]: https://cheatsheetseries.owasp.org/cheatsheets/Microservices_Security_Cheat_Sheet
[csnpm]: https://cheatsheetseries.owasp.org/cheatsheets/NPM_Security_Cheat_Sheet
[csnode]: https://cheatsheetseries.owasp.org/cheatsheets/Nodejs_Security_Cheat_Sheet
[csnodedocker]: https://cheatsheetseries.owasp.org/cheatsheets/NodeJS_Docker_Cheat_Sheet
[csphp]: https://cheatsheetseries.owasp.org/cheatsheets/PHP_Configuration_Cheat_Sheet
[csrest]: https://cheatsheetseries.owasp.org/cheatsheets/REST_Security_Cheat_Sheet
[csruby]: https://cheatsheetseries.owasp.org/cheatsheets/Ruby_on_Rails_Cheat_Sheet
[cssymfony]: https://cheatsheetseries.owasp.org/cheatsheets/Symfony_Cheat_Sheet
[cswebservice]: https://cheatsheetseries.owasp.org/cheatsheets/Web_Service_Security_Cheat_Sheet
[csxml]: https://cheatsheetseries.owasp.org/cheatsheets/XML_Security_Cheat_Shee
[csproactive-c2]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c2-leverage-security-frameworks-and-libraries
[control2]: https://owasp.org/www-project-proactive-controls/v3/en/c2-leverage-security-frameworks-libraries
[dependency]: https://owasp.org/www-project-dependency-check/
[edit060202]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/02-web-app-checklist/02-frameworks-libraries.md
[issue060202]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/02-web-app-checklist/02-frameworks-libraries
[proactive10]: https://owasp.org/www-project-proactive-controls/

\newpage
