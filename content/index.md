---
title: Pages
---

# Pages
{% assign static_files = site.static_files | where: "type", "pages" %}

{% for file in static_files %}
- [{{ file.name}}]({{ site.url }}{{ file.path}})
{% endfor %}
