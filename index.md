---
layout: page
title: ptcc's Blog!
tagline: A blog about frontend stuff (most of the time)
---

<ul class="posts">
  {% for post in site.posts %}
    <li><span class="pull-right">{{ post.date | date_to_string }}</span><a href="{{ BASE_PATH }}{{ post.url }}"><h2>{{ post.title }}</h2></a><br> {{ post.content | strip_html | truncatewords:20}}</li>
  {% endfor %}
</ul>

