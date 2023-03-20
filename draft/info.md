[Back to Project Homepage](/www-project-developer-guide/)

{% assign dev_file = site.static_files | where: "name", "devsite.txt" %}
{% if dev_file.size > 0 %}
{% assign site_base_url = '/' %}
{% else %}
{% assign site_base_url = '/www-project-developer-guide' %}
{% endif %}

### OWASP Developer Guide
{% assign pages = site.pages | where_exp: "page", "page.document contains 'OWASP Developer Guide'" | sort: 'order' | limit: 1000 %}
{% for p in pages %}

* {% if page.title == p.title %} {{p.title}} {% else %} {% unless p.url contains 'historical' %}[{{ p.title }}]({{site_base_url}}{{ p.url }}){% endunless %}{% endif %}
{% endfor %}