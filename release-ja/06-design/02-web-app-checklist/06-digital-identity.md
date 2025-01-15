---

title: Implement Digital Identity Checklist
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden, Andreas Happe
document: OWASP Developer Guide
order: 6260
permalink: /release/design/web_app_checklist/digital_identity/

---

{% include breadcrumb.html %}

### 4.2.6 Checklist: Implement Digital Identity

[Authentication][csauthn] is the process of verifying that an individual or entity is who they claim to be.
Session management is a process by which a server maintains the state of the users authentication
so that the user may continue to use the system without re-authenticating.

Refer to proactive control [C7: Implement Digital Identity][control7] and its [cheatsheets][csproactive-c6]
for more context from the OWASP Top 10 Proactive Controls project,
and use the list below as suggestions for a checklist that has been tailored for the individual project.

#### 1. Authentication

1. Design access control authentication thoroughly up-front
1. Force all requests to go through access control checks unless public
1. Do not hard code access controls that are role based
1. Log all access control events
1. Use [Multi-Factor Authentication][csmfa] (MFA) for sensitive or high value transactional accounts

#### 2. Passwords

1. Require authentication for all pages and resources, except those specifically intended to be public
1. All authentication controls must be enforced on a trusted system
1. Establish and utilize standard, tested, authentication services whenever possible
1. Use a centralized implementation for all authentication controls
1. Segregate authentication logic from the resource being requested and
    use redirection to and from the centralized authentication control
1. All authentication controls should fail securely
1. Administrative and account management must be at least as secure as the primary authentication mechanism
1. If your application manages a credential store, use cryptographically strong one-way salted hashes
1. Password hashing must be implemented on a trusted system
1. Validate the authentication data only on completion of all data input
1. Authentication failure responses should not indicate which part of the authentication data was incorrect
1. Utilize authentication for connections to external systems that involve sensitive information or functions
1. Authentication credentials for accessing services external to the application should be stored in a secure store
1. Use only HTTP POST requests to transmit authentication credentials
1. Only send non-temporary passwords over an encrypted connection or as encrypted data
1. Enforce password complexity and length requirements established by policy or regulation
1. Enforce account disabling after an established number of invalid login attempts
1. Password reset and changing operations require the same level of controls as account creation and authentication
1. Password reset questions are deprecated, see [Choosing and Using Security Questions Cheat Sheet][csquestions] as to why
1. If using email based resets, only send email to a pre-registered address with a temporary link/password
1. Temporary passwords and links should have a short expiration time
1. Enforce the changing of temporary passwords on the next use
1. Notify users when a password reset occurs
1. Prevent password re-use
1. The last use (successful or unsuccessful) of a user account should be reported to the user
    at their next successful login
1. Change all vendor-supplied default passwords and user IDs or disable the associated accounts
1. Re-authenticate users prior to performing critical operations
1. If using third party code for authentication inspect the code carefully
    to ensure it is not affected by any malicious code

#### 3. Cryptographic based authentication

1. Use the server or framework's session management controls
1. Session identifier creation must always be done on a trusted system
1. Session management controls should use well vetted algorithms that ensure sufficiently random session identifiers
1. Set the domain and path for cookies containing authenticated session identifiers
    to an appropriately restricted value for the site
1. Logout functionality should fully terminate the associated session or connection
1. Logout functionality should be available from all pages protected by authorization
1. Establish a session inactivity timeout that is as short as possible,
    based on balancing risk and business functional requirements
1. Disallow persistent logins and enforce periodic session terminations, even when the session is active
1. If a session was established before login, close that session and establish a new session after a successful login
1. Generate a new session identifier on any re-authentication
1. Do not allow concurrent logins with the same user ID
1. Do not expose session identifiers in URLs, error messages or logs
1. Implement appropriate access controls to protect server side session data
    from unauthorized access from other users of the server
1. Generate a new session identifier and deactivate the old one periodically
1. Generate a new session identifier if the connection security changes from HTTP to HTTPS,
    as can occur during authentication
1. Set the `secure` attribute for cookies transmitted over an [TLS][tls] connection
1. Set cookies with the `HttpOnly` attribute,
    unless you specifically require client-side scripts within your application to read or set a cookie value

#### References

* OWASP [Cheat Sheet: Authentication][csauthn]
* OWASP [Cheat Sheet: Choosing and Using Security Questions][csquestions]
* OWASP [Cheat Sheet: Forgot Password][csforgot]
* OWASP [Cheat Sheet: Multifactor Authentication][csmfa]
* OWASP [Cheat Sheet: Password Storage][cspass]
* OWASP [Cheat Sheet: Session Management][cssession]
* OWASP [Top 10 Proactive Controls][proactive10]

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue060206] or [edit on GitHub][edit060206].

[csproactive-c6]: https://cheatsheetseries.owasp.org/IndexProactiveControls.html#c6-implement-digital-identity
[control7]: https://top10proactive.owasp.org/the-top-10/c7-secure-digital-identities/
[csauthn]: https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet
[csmfa]: https://cheatsheetseries.owasp.org/cheatsheets/Multifactor_Authentication_Cheat_Sheet
[cspass]: https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet
[csforgot]: https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet
[cssession]: https://cheatsheetseries.owasp.org/cheatsheets/Session_Management_Cheat_Sheet
[csquestions]: https://cheatsheetseries.owasp.org/cheatsheets/Choosing_and_Using_Security_Questions_Cheat_Sheet
[edit060206]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/02-web-app-checklist/06-digital-identity.md
[issue060206]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/02-web-app-checklist/06-digital-identity
[proactive10]: https://top10proactive.owasp.org
[tls]: https://cheatsheetseries.owasp.org/cheatsheets/Transport_Layer_Security_Cheat_Sheet
