---
title: Pages
---

# Pages
{% assign static_files = site.static_files | where: "type", "pages" %}

{% for file in static_files %}
- [{{ file.name}}]({{ file.path | relative_url }})
{% endfor %}
