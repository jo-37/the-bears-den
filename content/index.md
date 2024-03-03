---
title: Pages
---

# Pages
{% assign static_files = site.static_files | where: "type", "pages" %}

{% for file in static_files %}
- [{{ file.name}}]({{ site.url }}{{ site.base_url }}{{ file.path}})
{% endfor %}
