---
title: jonesy archives
layout: default
---
  {% for post in site.posts %}
  <article>
    <p>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </p>
      <p>{{ post.excerpt }}</p>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
      <p>-------</p>
  </article>
{% endfor %}
