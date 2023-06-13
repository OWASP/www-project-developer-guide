---

title: Secure coding
layout: col-document
tags: OWASP Developer Guide
author: Shruti Kulkarni
contributors:
document: OWASP Developer Guide
order: 602

---

{% include breadcrumb.html %}

### 6.2 Secure coding

* Authentication
  * User
  * Server
  * Password policy
* Authorisation
  * Access control
  * Session management
  * JWT
  * SAML
* Input data validation
  * Identify input fields that form a SQL query. Check that these fields
      are suitably validated for type, format, length, and range.
  * To prevent SQL injection use bind variables in stored procedures and SQL statements.
      Also referred as prepared statements / parameterization of SQL statements.
      DO NOT concatenate strings that are an input to the database.
      The key is to ensure that raw input from end users is not accepted without sanitization.
      When converting data into a data structure (deserializing), perform explicit validation for all fields,
      ensuring that the entire object is semantically valid.
      Many technologies now come with data access layers that support input data validation.
      These layers are usually in the form of a library or a package. Ensure to add
      these libraries  / dependencies / packages to the project file such that they are not missed out.
  * Use a security vetted library for input data validation. Try not to use hard coded whitelist of characters.
      Validate all data from a centralised function / routine.
      In order to add a variable to a HTML context safely, use HTML entity encoding
      for that variable as you add it to a web template.
    * Validate HTTP headers. Dependencies that perform HTTP headers validation are available in technologies.
    * Validate post backs from javascript.
    * Validate data from http headers, input fields, hidden fields, drop down lists & other web components
    * Validate data retrieved from database. This will help mitigate persistent XSS.
    * Validate all redirects. Unvalidated redirects may lead to data / credential exfiltration.
        Evaluate any URL encodings before trying to use the URL.
    * Validate data received from redirects. The received data may be from untrusted source.
    * If any potentially hazardous characters must be allowed as input,
        be sure that you implement additional controls like output encoding,
        secure task specific APIs and accounting for  the utilization of that data throughout the application.
        Examples of common hazardous characters include: < > " ' % ( ) & + \ \' \"
    * If your standard validation routine cannot address the following inputs, then they should be checked discretely
      * Check for null bytes (%00)
      * Check for new line characters (%0d, %0a, \r, \n)
      * Check for “dot-dot-slash" (../ or ..\) path alterations characters.
          In cases where UTF-8 extended character set encoding is supported, address alternate representation like:
          `%c0%ae%c0%ae/`
          (Utilise canonicalization to address double encoding or other forms of obfuscation attacks)
    * Client-side storage (`localStorage`, `SessionStorage`, `IndexedDB`, WebSQL):
        If you use client-side storage for persistence of any variables,
        validate the date before consuming it in the application
    * Reject all input data that has failed validation.
    * If used, don’t involve user parameters in calculating the destination. This can usually be done.
        If destination parameters can’t be avoided, ensure that the supplied value is valid,
        and authorised for the user.
        It is recommended that any such destination parameters be a mapping value,
        rather than the actual URL or portion of the URL,
        and that server side code translate this mapping to the target URL.
        Applications can use ESAPI to override the `sendRedirect()` method
        to make sure all redirect destinations are safe.
* Output data encoding
  * If your code echos user input or URL parameters back to a Web page, validate input data as well as output data.
      It will help you prevent persistent as well as reflective cross-site scripting.
      Pay particular attention to areas of the application that permit users
      to modify configuration or personalization settings.
      Also pay attention to persistent free-form user input,
      such as message boards, forums, discussions, and Web postings.
      Encode javascript to prevent injection by escaping non-alphanumeric characters.
      Use quotation marks like " or ' to surround your variables.
      Quoting makes it difficult to change the context a variable operates in, which helps prevent XSS
  * Conduct all encoding on a trusted system (e.g., The server)
      Utilise a standard, tested routine for each type of outbound encoding
      Contextually output encode all data returned to the client
      that originated outside the application's trust boundary.
      HTML entity encoding is one example, but does not work in all cases
      Encode all characters unless they are known to be safe for the intended interpreter
      Contextually sanitise all output of untrusted data to queries for SQL, XML, and LDAP
      Sanitise all output of untrusted data to operating system commands
  * Output encoding is not always perfect. It will not always prevent XSS. Some contexts are not secure. These include:
      Callback functions
      Where URLs are handled in code such as this CSS `{ background-url : “javascript:alert(test)”; }`
      All JavaScript event handlers (`onclick()`, `onerror()`, `onmouseover()`).
      Unsafe JavaScript functions like `eval()`, `setInterval()`, `setTimeout()`
      Don't place variables into these contexts as even with output encoding, it will not prevent an XSS attack fully
  * Do not rely on client-side validation. Perform validation on server side to prevent second order attacks.
* Canonicalisation
  * Convert all input data to an accepted/decided format like UTF-8.  This will help prevent spoofing of character
* Test all URLs with different parameter values.
    Spider and check the site/product/application/portal for redirects.
* Connection with backend
    Assign required permissions and privileges for accounts / roles
    used by the application to connect to the database.
    In the event of any compromise of the account / role,
    the malicious actor would be able to do whatever the account /role has permissions for.
* Insecure direct object references
* Unvalidated redirects
    Test all URLs with different parameter values to validate any redirects
    If used, do not allow the URL as user input for the destination.
    Where possible, have the user provide short name, ID or token which is mapped server-side to a full target URL.
    This provides the protection against the URL tampering attack.
    Be careful that this doesn't introduce an enumeration vulnerability where
    a user could cycle through IDs to find all possible redirect targets
    If user input can’t be avoided, ensure that the supplied value is valid, appropriate for the application,
    and is authorised for the user.
    Sanitise input by creating a list of trusted URLs (lists of hosts or a regex).
    This should be based on an allow-list approach, rather than a block list.
    Force all redirects to first go through a page notifying users that they are going off of your site,
    with the destination clearly displayed, and have them click a link to confirm.
* JSON
    For JSON, verify that the Content-Type header is application/json and not text/html to prevent XSS
    Do not use duplicate keys. Usage of duplicate keys may be processed differently by parsers.
    For example last-key precedence versus first-key precedence.
* Generate fatal parse errors on duplicate keys.
    Do not perform character truncation. Instead, replace invalid Unicode with placeholder characters
    (e.g., unpaired surrogates should be displayed as the Unicode replacement character `U+FFFD`).
    Truncating may break sanitization routines for multi-parser applications."
* Produce errors when handling integers or floating-point numbers that cannot be represented faithfully
* Do not use `eval()` with JSON. This opens up for JSON injection attacks. Use JSON.parse() instead
    Data from an untrusted source is not sanitised by the server and written directly to a JSON stream.
    This is referred to as server-side JSON injection.
    Data from an untrusted source is not sanitised and parsed directly using the JavaScript `eval` function.
    This is referred to as client-side JSON injection.
    To prevent server-side JSON injections, sanitise all data before serialising it to JSON
    Escape characters like ":", "\", "@", "'”", "%", "?", "--", ">", "<", "&"

### JSON Vulnerability Protection

A JSON vulnerability allows third party website to turn your JSON resource URL into JSONP request under some conditions.
To counter this your server can prefix all JSON requests with following string "")]}',\n"".
AngularJS will automatically strip the prefix before processing it as JSON.

For example if your server needs to return: `['one','two']`
which is vulnerable to attack, your server can return: `)]}', ['one','two']`

Refer to [JSON vulnerability protection](https://docs.angularjs.org/api/ng/service/$http#json-vulnerability-protection)
Always have the outside primitive be an object for JSON strings

Exploitable: `[{""object"": ""inside an array""}]`

Not exploitable: `{""object"": ""not inside an array""}`

Also not exploitable: `{""result"": [{""object"": ""inside an array""}]}"`

* Avoid manual build of JSON, use an existing framework
* Ensure calling function does not convert JSON into a javascript
    and JSON returns its response as a non-array json object
* Wrap JSON in () to force the interpreter to think of it as JSON and not a code block
* When using node.js, on the server use a proper JSON serializer to encode user-supplied data properly
    to prevent the execution of user-supplied input on the browser.

\newpage
