---

title: Implement Digital Identity Checklist
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 626
permalink: /release/design/web_app_checklist/digital_identity/

---

{% include breadcrumb.html %}

### 4.2.6 Checklist: Implement Digital Identity

Authentication is the process of verifying that an individual or entity is who they claim to be.
Session management is a process by which a server maintains the state of the users authentication
so that the user may continue to use the system without re-authenticating.

Refer to proactive control [C6: Implement Digital Identity][control6]
for more context from the OWASP Top 10 Proactive Controls project,
and use the checklists below as suggestions for the checklist that has been tailored for the individual project.

#### Authentication

* Design access control authentication thoroughly up-front
* Force all requests to go through access control checks unless public
* Do not hard code access controls that are role based
* Log all access control events
* Use Multi-Factor Authentication for highly sensitive or high value transactional accounts

#### Passwords

* Require authentication for all pages and resources, except those specifically intended to be public
* All authentication controls must be enforced on a trusted system
* Establish and utilize standard, tested, authentication services whenever possible
* Use a centralized implementation for all authentication controls
* Segregate authentication logic from the resource being requested and
    use redirection to and from the centralized authentication control
* All authentication controls should fail securely
* Administrative and account management must be at least as secure as the primary authentication mechanism
* If your application manages a credential store, use cryptographically strong one-way salted hashes
* Password hashing must be implemented on a trusted system
* Validate the authentication data only on completion of all data input
* Authentication failure responses should not indicate which part of the authentication data was incorrect
* Utilize authentication for connections to external systems that involve sensitive information or functions
* Authentication credentials for accessing services external to the application should be stored in a secure store
* Use only HTTP POST requests to transmit authentication credentials
* Only send non-temporary passwords over an encrypted connection or as encrypted data
* Enforce password complexity and length requirements established by policy or regulation
* Enforce account disabling after an established number of invalid login attempts
* Password reset and changing operations require the same level of controls as account creation and authentication
* Password reset questions should support sufficiently random answers
* If using email based resets, only send email to a pre-registered address with a temporary link/password
* Temporary passwords and links should have a short expiration time
* Enforce the changing of temporary passwords on the next use
* Notify users when a password reset occurs
* Prevent password re-use
* The last use (successful or unsuccessful) of a user account should be reported to the user
    at their next successful login
* Change all vendor-supplied default passwords and user IDs or disable the associated accounts
* Re-authenticate users prior to performing critical operations
* If using third party code for authentication inspect the code carefully
    to ensure it is not affected by any malicious code

#### Cryptographic based authentication

* Use the server or framework's session management controls
* Session identifier creation must always be done on a trusted system
* Session management controls should use well vetted algorithms that ensure sufficiently random session identifiers
* Set the domain and path for cookies containing authenticated session identifiers
    to an appropriately restricted value for the site
* Logout functionality should fully terminate the associated session or connection
* Logout functionality should be available from all pages protected by authorization
* Establish a session inactivity timeout that is as short as possible,
    based on balancing risk and business functional requirements
* Disallow persistent logins and enforce periodic session terminations, even when the session is active
* If a session was established before login, close that session and establish a new session after a successful login
* Generate a new session identifier on any re-authentication
* Do not allow concurrent logins with the same user ID
* Do not expose session identifiers in URLs, error messages or logs
* Implement appropriate access controls to protect server side session data
    from unauthorized access from other users of the server
* Generate a new session identifier and deactivate the old one periodically
* Generate a new session identifier if the connection security changes from HTTP to HTTPS,
    as can occur during authentication
* Set the `secure` attribute for cookies transmitted over an TLS connection
* Set cookies with the `HttpOnly` attribute,
    unless you specifically require client-side scripts within your application to read or set a cookie value

#### References

* OWASP [Cheat Sheet: Authentication][csauth]
* OWASP [Cheat Sheet: Password Storage][cspass]
* OWASP [Cheat Sheet: Forgot Password][csforgot]
* OWASP [Cheat Sheet: Session Management][cssession]
* OWASP [Top 10 Proactive Controls][proactive10]

----


[control6]: https://owasp.org/www-project-proactive-controls/v3/en/c6-digital-identity
[csauth]: https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html
[cspass]: https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet.html
[csforgot]: https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet.html
[cssession]: https://cheatsheetseries.owasp.org/cheatsheets/Session_Management_Cheat_Sheet.html
[proactive10]: https://owasp.org/www-project-proactive-controls/

\newpage
