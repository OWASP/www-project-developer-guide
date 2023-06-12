---

title: Security Requirements Introduction
layout: col-document
tags: OWASP Developer Guide
author: Shruti Kulkarni
contributors:
document: OWASP Developer Guide
order: 501

---

{% include breadcrumb.html %}

### 5.1 Introduction to security requirements

The OWASP Development Guide is being rewritten by the OWASP community.
and the content of this section has yet to be filled in.

If you would like to contribute then follow the
[contributing guidelines](https://github.com/OWASP/www-project-developer-guide/blob/main/contributing.md)
and submit your content for review.

The following subsections are planned:

* Threat modeling (hive off to threat modeling material on OWASP)
* Regulatory / statutory requirements

* Input data validation:
* Identify input fields that form a SQL query. Check that these fields are suitably validated for type, format, length, and range.
* To prevent SQL injection use bind variables in stored procedures and SQL statements. 
Also referred as prepared statements / parametrisation of SQL statements. DO NOT concatenate strings that are an input to the database.

The key is to ensure that raw input from end users is not accepted without sanitisation.

When converting data into a data structure (deserialising), perform explicit validation for all fields, ensuring that the entire object is semantically valid.

Many technologies now come with data access layers that support input data validation. These layers are usually in the form of a library or a package. Ensure to add these libraries / dependencies / packages to the project file such that they are not missed out.   

* Use a security vetted library for input data validation. Try not to use hardcoded whitelist of characters. Validate all data from a centralised function / routine.

In order to add a variable to a HTML context safely, use HTML entity encoding for that variable as you add it to a web template.

* Validate HTTP headers. Dependencies that perform HTTP headers validation are available in technologies.
* Validate post backs from javascript. 
* Validate data from http headers, input fields, hidden fields, drop down lists & other web components
* Validate data retrieved from database. This will help mitigate persistent XSS.
* Validate all redirects. Unvalidated redirects may lead to data / credential exfiltration. Evaluate any URL encodings before trying to use the URL.
* Validate data received from redirects. The received data may be from untrusted source.
* If any potentially hazardous characters must be allowed as input, be sure that you implement additional controls like output encoding, secure task specific APIs and accounting for the utilizationof that data throughout the application. Examples of common hazardous characters include: < > " ' % ( ) & + \ \' \"
* If your standard validation routine cannot address the following inputs, then they should be checked
discretely
        o Check for null bytes (%00)
        o Check for new line characters (%0d, %0a, \r, \n)
        o Check for “dot-dot-slash" (../ or ..\) path alterations characters. In cases where UTF-8 extended character set encoding is supported, address alternate representation like:     %c0%ae%c0%ae/
        (Utilise canonicalisation to address double encoding or other forms of obfuscation attacks)
        
* Client-side storage (localStorage,SessionStorage, IndexedDB, WebSQL): If you use client-side storage for persistence of any variables, validate the date before consuming it in the application
* If your code echos user input or URL parameters back to a Web page, validate input data as well as output data.
It will help you prevent persistent as well as reflective cross-site scripting.  

Pay particular attention to areas of the application that permit users to modify configuration or personalisation settings. 
Also pay attention to persistent free-form user input, such as message boards, forums, discussions, and Web postings.

Encode javascript to prevent injection by escaping non-alphanumeric characters. Use quotation marks like " or ' to surround your variables. Quoting makes it difficult to change the context a variable operates in, which helps prevent XSS

* Conduct all encoding on a trusted system (e.g., The server)
 - Utilise a standard, tested routine for each type of outbound encoding
 - Contextually output encode all data returned to the client that originated outside the application's trust boundary. HTML entity encoding is one example, but does not work in all cases
 - Encode all characters unless they are known to be safe for the intended interpreter
 - Contextually sanitise all output of un-trusted data to queries for SQL, XML, and LDAP
 - Sanitise all output of un-trusted data to operating system commands

* Output encoding is not always perfect. It will not always prevent XSS. Some contexts are not secure. These include:
 - Callback functions
 - Where URLs are handled in code such as this CSS { background-url : “javascript:alert(test)”; }
 - All JavaScript event handlers (onclick(), onerror(), onmouseover()).
 - Unsafe JavaScript functions like eval(), setInterval(), setTimeout()
Don't place variables into these contexts as even with output encoding, it will not prevent an XSS attack fully.

* Assign required permissions and privileges for accounts / roles used by the application to connect to the database. In the event of any compromise of the account / role, the malicious actor would be able to do whatever the account /role has permissions for. 

* Do not rely on client-side validation. Perform validation on server side to prevent second order attacks.

* Convert all input data to an accepted/decided format like UTF-8. 
This will help prevent spoofing of characters

* Reject all input data that has failed validation.

* If used, don’t involve user parameters in calculating the destination. This can usually be done.
If destination parameters can’t be avoided, ensure that the supplied value is valid, and authorised for the user.It is recommended that any such destination parameters be a mapping value, rather than the actual URL or portion of the URL, and that server side code translate this mapping to the target URL. Applications can use ESAPI to override the sendRedirect() method to make sure all redirect destinations are safe.

* Test all URLs with different parameter values.
Spider and check the site/product/application/portal for redirects.
\newpage
