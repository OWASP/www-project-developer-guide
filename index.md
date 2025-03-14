---

layout: col-sidebar
title: OWASP Developer Guide
tags: dev-guide, developer guide
level: 3
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

<style type="text/css">
.image-right {
  height: 180px;
  display: block;
  margin-left: auto;
  margin-right: auto;
  float: right;
}
</style>

![Developer Guide](assets/images/dg_logo.png "OWASP Developer Guide"){: .image-right }

The [OWASP Developer Guide](release) provides an introduction to security concepts
and a handy reference for application and system developers.

This guide does not seek to replicate the many excellent sources on specific security topics;
it rarely tries to go into detail on a subject and instead provides links for greater depth on these security topics.

The content of the Developer Guide aims to be accessible, introducing practical security concepts
and providing enough detail to get developers started on various OWASP tools and documents.

The intended audience of the Developer Guide is application developers working in various domains
such as web, desktop, mobile, API and cloud.

### History

Along with the OWASP Top Ten, the Developer Guide is one of the original resources
published soon after OWASP was formed in 2001.
Version 1.0 of the Developer Guide was released in 2002
and then there were various [updates][versions] culminating in version 2.0 in 2005.
After discussions and iterations throughout 2023 and 2024, the Developer Guide has now been updated
for the modern security landscape using contributions from the wider application security community.

Periodically the draft version is tagged and the contents promoted to the [release area](release) of the Developer Guide.
The [draft version](draft) is a work in progress and is subject to large scale and frequent changes.

### Contributing

Contributions and suggestions are all welcome, we just ask that you follow our [code of conduct][conduct]
and read the [contributing guidelines][contribution] which provide style and document structure suggestions.
We also welcome [new issues][issues], changes via a [pull request][request]
and discussions in the [project wiki][wiki].

The easiest way to get in contact with the development community for this documentation project
is via the OWASP Slack [#project-developer-guide][project] project channel (you may need to [subscribe][slack] first).

----

OWASP DevGuide: _accessible security for developers_

[conduct]: code_of_conduct.md
[contribution]: contributing.md
[issues]: https://github.com/OWASP/www-project-developer-guide/issues/new/choose
[project]: https://owasp.slack.com/messages/C04QN6CMNAC
[slack]: https://owasp.org/slack/invite
[request]: https://github.com/OWASP/www-project-developer-guide/pulls
[versions]: https://github.com/OWASP/DevGuide/wiki#old-versions
[wiki]: https://github.com/OWASP/www-project-developer-guide/wiki
