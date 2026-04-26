---
layout: default
title: Categories
permalink: /categories/
---

<div class="home">
  <h1 class="page-heading">Categories</h1>

  {% assign categories = site.categories | sort %}
  <ul>
    {% for category in categories %}
      {% capture category_url %}/categories/{{ category[0] | slugify }}/{% endcapture %}
      <li>
        <a href="{{ category_url | relative_url }}">{{ category[0] }}</a>
        ({{ category[1].size }})
      </li>
    {% endfor %}
  </ul>
</div>