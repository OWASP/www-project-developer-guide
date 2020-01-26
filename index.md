---

layout: col-sidebar
title: OWASP [GROUPNAME]
tags: example-tag
level: 4
type: example
auto-migrated: 

---

* {{ site.url }}
* {{ page.url }}
* {{ site.github.url }}
* {{site.github.url | replace: 'www2.', ''}}{{page.url}}

<!-- rebuild 9 -->
This is an example of a Project or Chapter Page.  Please change these items to indicate the actual information you wish to present.  In addition to this information, the 'front-matter' above this text should be modified to reflect your actual information.  An explanation of each of the front-matter items is below:

layout: This is the layout used by project and chapter pages.  You should leave this value as col-sidebar

title: This is the title of your project or chapter page, usually the name.  For example, OWASP Zed Attack Proxy or OWASP Baltimore

tags: This is a space-delimited list of tags you associate with your project or chapter.  If you are using tabs, at least one of these tags should be unique in order to be used in the tabs files (an example tab is included in this repo) 

level: For projects, this is your project level (2 - Incubator, 3 - Lab, 4 - Flagship)

type: For projects, one of documentation, code, or tool

A good resource for github markdown tags can be found [here]([https://www2.owasp.org/migration)

### List of Donors
{% assign donors = site.data.ow_attributions | uniq %}
{% for donor in donors %}
* {{ donor | strip }}
{% endfor %}
