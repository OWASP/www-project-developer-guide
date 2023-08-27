---

title: Leverage Security Frameworks and Libraries Checklist
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 2003

---

{% include breadcrumb.html %}

### 20.3 Checklist: Leverage Security Frameworks and Libraries

![Developer Guide](../assets/images/dg_wip.png "OWASP Developer Guide"){: height="220px" }

The OWASP Development Guide is being rewritten by the OWASP community,
and the content has yet to be filled in for section 'C2: Leverage Security Frameworks and Libraries'.

If you would like to contribute then follow the [contributing guidelines][contribute]
and submit your content for review.

[contribute]: https://github.com/OWASP/www-project-developer-guide/blob/main/contributing.md

## Memory management

- [ ]   Utilize input and output controls for untrusted data

- [ ]   Check that the buffer is as large as specified

- [ ]   When using functions that accept a number of bytes ensure that NULL termination is handled correctly

- [ ]   Check buffer boundaries if calling the function in a loop and protect against overflow

- [ ]   Truncate all input strings to a reasonable length before passing them to other functions

- [ ]   Specifically close resources, don't rely on garbage collection

- [ ]   Use non-executable stacks when available

- [ ]   Avoid the use of known vulnerable functions

- [ ]   Properly free allocated memory upon the completion of functions and at all exit points

- [ ]   Overwrite any sensitive information stored in allocated memory at all exit points from the function

## General coding practices

- [ ]   Use tested and approved managed code rather than creating new unmanaged code for common tasks

- [ ]   Utilize task specific built-in APIs to conduct operating system
    tasks. Do not allow the application to issue commands directly to
    the Operating System, especially through the use of application
    initiated command shells

- [ ]   Use checksums or hashes to verify the integrity of interpreted code,
    libraries, executables, and configuration files

- [ ]   Utilize locking to prevent multiple simultaneous requests or use a
    synchronization mechanism to prevent race conditions

- [ ]   Protect shared variables and resources from inappropriate concurrent
    access

- [ ]   Explicitly initialize all your variables and other data stores,
    either during declaration or just before the first usage

- [ ]   In cases where the application must run with elevated privileges,
    raise privileges as late as possible, and drop them as soon as
    possible

- [ ]   Avoid calculation errors by understanding your programming language\'s underlying representation

- [ ]   Do not pass user supplied data to any dynamic execution function

- [ ]   Restrict users from generating new code or altering existing code

- [ ]   Review all secondary applications, third party code and libraries to
    determine business necessity and validate safe functionality

- [ ]   Implement safe updating using encrypted channels

\newpage
