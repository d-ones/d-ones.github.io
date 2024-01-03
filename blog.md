---
title: jonesy archives
layout: default
---

<div>
    <a href="/feed.xml" target="_blank">RSS</a>
    <p>--</p>
    {% for post in site.posts %}
    <article>
        <p>
        <a href="{{ post.url }}">
            {{ post.title }}
        </a>
        </p>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
      <p>--</p>
  </article>
{% endfor %}
</div>
