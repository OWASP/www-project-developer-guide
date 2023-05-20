---

layout: col-sidebar
title: OWASP Developer Guide
tags: dev-guide, developer guide
level: 2
type: documentation
pitch: The Developer Guide allows businesses, developers, designers
       and solution architects to produce secure web applications.
       If done from the earliest stages, secure
       applications cost about the same to develop as insecure applications,
       but are far more cost effective in the long run.

---
{% assign dev_file = site.static_files | where: "name", "devsite.txt" %}
{% if dev_file.size > 0 %}
{% assign site_base_url = '/' %}
{% else %}
{% assign site_base_url = site.github.url | replace: 'owasp.github.io','owasp.org' | replace: 'http://', 'https://' %}
{% endif %}

Along with the OWASP Top Ten, the Developer Guide is one of the original resources
published soon after OWASP was formed in 2001.

Version 1.0 of the Developer Guide was released in 2002
and since then there have been various [releases][versions], the latest being version 2.0 in 2005.
There is a [draft version](draft) available that is based on an unreleased version (3.0) from 2015.
This is very much work in progress and is subject to large scale and frequent changes.

The Developer Guide needs to be updated for the modern security landscape,
and OWASP is reviving this project to do just that.
The project has a team of leaders that will oversee the project
and now we need as many members of the security community as possible to contribute.

### Contributing
Contributions and suggestions are all welcome, we just ask that you follow our [code of conduct][conduct].
Contributors can [make suggestions][issues], provide changes via a [pull request][request]
or discuss topics in the [project wiki][wiki].

The easiest way to get in contact with the development community for this documentation project
is via the OWASP Slack [#project-developer-guide][project] project channel.

[conduct]: CODE_OF_CONDUCT.md
[issues]: https://github.com/OWASP/www-project-developer-guide/issues/new/choose
[project]: https://owasp.slack.com/messages/C04QN6CMNAC
[request]: https://github.com/OWASP/www-project-developer-guide/pulls
[versions]: https://github.com/OWASP/DevGuide/wiki#old-versions
[wiki]: https://github.com/OWASP/www-project-developer-guide/wiki
