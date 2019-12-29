---
permalink: /tasting_notes_EN/
---

{% assign Scotches = site.categories.EN | where_exp: "post", "post.categories contains 'Scotch'" %}

<ul>
  {% for post in Scotches %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>