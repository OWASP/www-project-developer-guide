---

title: Memory Management
layout: col-document
tags: OWASP Developer Guide
author: Shruti Kulkarni
contributors:
document: OWASP Developer Guide
order: 608

---

{% include breadcrumb.html %}
### 6.8 Memory Management

* Check that the buffer is as large as specified

* When using functions that accept a number of bytes to copy, such as strncpy( ), be aware that if the destination buffer size is equal to the source buffer size, it may not NULL-terminate the string

* Check buffer boundaries if calling the function in a loop and make sure there is no danger of writing past the allocated space

* Truncate all input strings to a reasonable length before passing them to the copy and concatenation functions

* Specifically close resources, do not rely on garbage collection. (for example connection objects, file handles, etc.)

* Properly free allocated memory upon the completion of functions and at all exit points.


\newpage
