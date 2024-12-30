---

title: Memory Management
layout: col-document
tags: OWASP Developer Guide
contributors: Roxana Calderon, Shruti Kulkarni
document: OWASP Developer Guide
order: 54180
permalink: /release-es/appendices/implementation_dos_donts/memory_management/

---

{% include breadcrumb.html %}

### 12.1.8 Memory Management

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

Traducción de versión [original en inglés][release140108].

[edit140108]: https://github.com/OWASP/www-project-developer-guide/blob/main/release/14-appendices/01-implementation-dos-donts/08-memory-management.md


\newpage
