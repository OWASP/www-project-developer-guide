---

title: Memory Management
layout: col-document
tags: OWASP Developer Guide
author: Shruti Kulkarni
document: OWASP Developer Guide
order: 608

---

{% include breadcrumb.html %}

### 6.8 Memory Management

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

The OWASP Developer Guide is a community effort; if you see something that needs changing
then [submit an issue][issue0608] or a [pull request][pr] .

[issue0608]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-secure-design/08-memory-management
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls

\newpage
