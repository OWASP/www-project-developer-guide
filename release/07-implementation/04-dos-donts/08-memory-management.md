---

title: Memory Management
layout: col-document
tags: OWASP Developer Guide
contributors: Shruti Kulkarni
document: OWASP Developer Guide
order: 7480
permalink: /release/implementation/dos_donts/memory_management/

---

{% include breadcrumb.html %}

### 5.4.8 Memory Management

Here is a collection of Do's and Don'ts when it comes to memory management, gathered from practical experiences.

* Check that the buffer is as large as specified
* When using functions that accept a number of bytes to copy, such as `strncpy()`,
    be aware that if the destination buffer size is equal to the source buffer size,
    it may not NULL-terminate the string
* Check buffer boundaries if calling the function in a loop and make sure there is no danger
    of writing past the allocated space
* Truncate all input strings to a reasonable length before passing them to the copy and concatenation functions
* Specifically close resources, do not rely on garbage collection. (for example connection objects, file handles, etc.)
* Properly free allocated memory upon the completion of functions and at all exit points.

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue070408] or [edit on GitHub][edit070408].

[issue070408]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2007-implementation/04-dos-donts/08-memory-management
[edit070408]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/07-implementation/04-dos-donts/08-memory-management.md
