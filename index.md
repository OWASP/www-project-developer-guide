---

layout: col-sidebar
title: OWASP Developer Guide
tags: dev-guide, developer guide
level: 2
type: documentation
pitch: The Developer Guide allows businesses, developers, designers and solution architects to produce secure web applications. If done from the earliest stages, secure   
       applications cost about the same to develop as insecure applications, but are far more cost effective in the long run. 
auto-migrated: 

---
{% assign dev_file = site.static_files | where: "name", "devsite.txt" %}
{% if dev_file.size > 0 %}
{% assign site_base_url = '/' %}
{% else %}
{% assign site_base_url = site.github.url | replace: 'owasp.github.io','owasp.org' | replace: 'http://', 'https://' %}
{% endif %}

Site base url: {{site_base_url}}

This is an example of a Project or Chapter Page.  Please change these items to indicate the actual information you wish to present.  In addition to this information, the 'front-matter' above this text should be modified to reflect your actual information.  An explanation of each of the front-matter items is below:

layout: This is the layout used by project and chapter pages.  You should leave this value as col-sidebar

title: This is the title of your project or chapter page, usually the name.  For example, OWASP Zed Attack Proxy or OWASP Baltimore

tags: This is a space-delimited list of tags you associate with your project or chapter.  If you are using tabs, at least one of these tags should be unique in order to be used in the tabs files (an example tab is included in this repo) 

level: For projects, this is your project level (2 - Incubator, 3 - Lab, 4 - Flagship)

type: For projects, one of documentation, code, or tool

A good resource for github markdown tags can be found [here](https://owasp.org/migration)

### List of Donors
{% assign donors = site.data.ow_attributions | uniq %}
{% for donor in donors %}
* {{ donor | strip }}
{% endfor %}
