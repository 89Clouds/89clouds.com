---
layout: page
title: Blog
---
{% include JB/setup %}

## Welcome to 89 Clouds Labs!

### Here's what's been going on:

<ul class="posts unstyled">
  {% for post in site.posts limit:10 %}
    <li>
      <span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
    </li>
    <div class="synopsis">
      <p>{{ post.synopsis }} <a href="{{ BASE_PATH }}{{ post.url }}">&raquo;</a></p>
    </div>
  {% endfor %}
</ul>
