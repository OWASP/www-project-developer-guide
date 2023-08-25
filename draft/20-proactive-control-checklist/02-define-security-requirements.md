---

title: Define Security Requirements Checklist
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 2002

---

{% include breadcrumb.html %}

### 20.2 Checklist: Define Security Requirements

![Developer Guide](../assets/images/dg_wip.png "OWASP Developer Guide"){: height="220px" }

The OWASP Development Guide is being rewritten by the OWASP community,
and the content has yet to be filled in for section 'C1: Define Security Requirements'.

If you would like to contribute then follow the [contributing guidelines][contribute]
and submit your content for review.

[contribute]: https://github.com/OWASP/www-project-developer-guide/blob/main/contributing.md

## System configuration

- [ ]   Ensure servers, frameworks and system components are running the latest approved version

- [ ]   Ensure servers, frameworks and system components have all patches issued for the version in use

- [ ]   Turn off directory listings

- [ ]   Restrict the web server, process and service accounts to the least privileges possible

- [ ]   When exceptions occur, fail securely

- [ ]   Remove all unnecessary functionality and files

- [ ]   Remove test code or any functionality not intended for production, prior to deployment

- [ ]   Prevent disclosure of your directory structure in the robots.txt
    file by placing directories not intended for public indexing into
    an isolated parent directory

- [ ]   Define which HTTP methods, Get or Post, the application will support
    and whether it will be handled differently in different pages in
    the application

- [ ]   Disable unnecessary HTTP methods

- [ ]   If the web server handles different versions of HTTP ensure that they
    are configured in a similar manner and ensure any differences are understood

- [ ]   Remove unnecessary information from HTTP response headers related to
    the OS, web-server version and application frameworks

- [ ]   The security configuration store for the application should be able
    to be output in human readable form to support auditing

- [ ]   Implement an asset management system and register system components
    and software in it

- [ ]   Isolate development environments from the production network and
    provide access only to authorized development and test groups

- [ ]   Implement a software change control system to manage and record
    changes to the code both in development and production

## File management

- [ ]   Do not pass user supplied data directly to any dynamic include function

- [ ]   Require authentication before allowing a file to be uploaded

- [ ]   Limit the type of files that can be uploaded to only those types
    that are needed for business purposes

- [ ]   Validate uploaded files are the expected type by checking file
    headers rather than by file extension

- [ ]   Do not save files in the same web context as the application

- [ ]   Prevent or restrict the uploading of any file that may be
    interpreted by the web server.

- [ ]   Turn off execution privileges on file upload directories

- [ ]   Implement safe uploading in UNIX by mounting the targeted file
    directory as a logical drive using the associated path or the
    chrooted environment

- [ ]   When referencing existing files, use an allow-list of allowed file names and types

- [ ]   Do not pass user supplied data into a dynamic redirect

- [ ]   Do not pass directory or file paths, use index values mapped to pre-defined list of paths

- [ ]   Never send the absolute file path to the client

- [ ]   Ensure application files and resources are read-only

- [ ]   Scan user uploaded files for viruses and malware


\newpage
