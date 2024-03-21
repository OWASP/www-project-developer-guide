---

title: Enforce Access Controls Checklist
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 6270
permalink: /release/design/web_app_checklist/access_controls/

---

{% include breadcrumb.html %}

### 4.2.7 Checklist: Enforce Access Controls

Access Control (or Authorization) is the process of granting or denying specific requests
from a user, program, or process.

Refer to proactive control [C7: Enforce Access Controls][control7]
for more context from the OWASP Top 10 Proactive Controls project,
and use the checklists below as suggestions for the checklist that has been tailored for the individual project.

#### Authorization

* Design access control / authorization thoroughly up-front
* Force all requests to go through access control checks unless public
* Deny by default; if a request is not specifically allowed then it is denied
* Apply least privilege, providing the least access as is necessary
* Log all authorization events

#### Access control

* Enforce authorization controls on every request
* Use only trusted system objects for making access authorization decisions
* Use a single site-wide component to check access authorization
* Access controls should fail securely
* Deny all access if the application cannot access its security configuration information
* Segregate privileged logic from other application code
* Limit the number of transactions a single user or device can perform in a given period of time,
    low enough to deter automated attacks but above the actual business requirement
* If long authenticated sessions are allowed, periodically re-validate a user's authorization
* Implement account auditing and enforce the disabling of unused accounts
* The application must support termination of sessions when authorization ceases

#### References

* OWASP [Cheat Sheet: Authorization][csaz]
* OWASP [Top 10 Proactive Controls][proactive10]

----

[control7]: https://owasp.org/www-project-proactive-controls/v3/en/c7-enforce-access-controls
[csaz]: https://cheatsheetseries.owasp.org/cheatsheets/Authorization_Cheat_Sheet.html
[proactive10]: https://owasp.org/www-project-proactive-controls/
