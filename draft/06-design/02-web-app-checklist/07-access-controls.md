---

title: Enforce Access Controls Checklist
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 627
permalink: /draft/design/web_app_checklist/access_controls/

---

{% include breadcrumb.html %}

### 4.2.7 Checklist: Enforce Access Controls

Access Control or [Authorization][csauthz] is the process of granting or denying specific requests
from a user, program, or process.

Refer to proactive control [C7: Enforce Access Controls][control7] and its [cheatsheets][cheatsheet-proactive-c7]
for more context from the OWASP Top 10 Proactive Controls project,
and use the list below as suggestions for a checklist that has been tailored for the individual project.

#### 1. Authorization

1. Design access control / authorization thoroughly up-front
1. Force all requests to go through access control checks unless public
1. Deny by default; if a request is not specifically allowed then it is denied
1. Apply least privilege, providing the least access as is necessary
1. Log all authorization events

#### 2. Access control

1. Enforce authorization controls on every request
1. Use only trusted system objects for making access authorization decisions
1. Use a single site-wide component to check access authorization
1. Access controls should fail securely
1. Deny all access if the application cannot access its security configuration information
1. Segregate privileged logic from other application code
1. Limit the number of transactions a single user or device can perform in a given period of time,
    low enough to deter automated attacks but above the actual business requirement
1. If long authenticated sessions are allowed, periodically re-validate a user's authorization
1. Implement account auditing and enforce the disabling of unused accounts
1. The application must support termination of sessions when authorization ceases

#### References

* OWASP [Cheat Sheet: Authorization][csauthz]
* OWASP [Top 10 Proactive Controls][proactive10]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue060207] or [edit on GitHub][edit060207].

[cheatsheet-proactive-c7]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c7-enforce-access-controls
[control7]: https://owasp.org/www-project-proactive-controls/v3/en/c7-enforce-access-controls
[csauthz]: https://cheatsheetseries.owasp.org/cheatsheets/Authorization_Cheat_Sheet.html
[edit060207]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/02-web-app-checklist/07-access-controls.md
[issue060207]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/02-web-app-checklist/07-access-controls
[proactive10]: https://owasp.org/www-project-proactive-controls/

\newpage
