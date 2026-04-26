---
layout: default
title: Blog
permalink: /blog/
---

<div class="home">
  <h1 class="page-heading">Blog</h1>

  {% assign excluded_categories = "notes,private" | split: "," %}

  <ul class="post-list">
    {% for post in site.posts %}
      {% assign hide_post = false %}

      {% for excluded in excluded_categories %}
        {% if post.categories contains excluded %}
          {% assign hide_post = true %}
        {% endif %}
      {% endfor %}

      {% unless hide_post %}
        <li>
          {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
          <span class="post-meta">{{ post.date | date: date_format }}</span>
          <h3>
            <a class="post-link" href="{{ post.url | relative_url }}">
              {{ post.title | escape }}
            </a>
          </h3>

          {% if site.show_excerpts %}
            {{ post.excerpt }}
          {% endif %}
        </li>
      {% endunless %}
    {% endfor %}
  </ul>
</div>