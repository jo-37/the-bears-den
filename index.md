---
title: The Bear's Den
---

# Posts

<table>
  <tr>
    <th>Date</th>
    <th>Title</th>
  </tr>
  {% for post in site.posts %}
  <tr>
    <td>
    {{ post.date | date_to_long_string }}
    </td>
    <td>
    <a href="{{ post.url | relative_url }}">
		{{ post.title}}
	</a>
    </td>
  </tr>
  {% endfor %}
</table>
