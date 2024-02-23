---
title: The Bear's Den
---

# Posts

```html
<table>
  <th>
    <td>Date</td>
    <td>Title</td>
  </th>
  {% for post in site.posts %}
  <tr>
    <td>
    {{ post.date | date_to_long_string }}
    </td>
    <td>
    [{{ post.title}}]({{ post.url | relative_url }})
    </td>
  </tr>
  {% endfor %}
</table>
```
