---
layout: page
title: List of all blog posts
exclude_from_nav: true
---

{% for post in site.posts %}
  <ul>
    <li>
      <a href="{{ post.url | remove: 'index.html' }}">{{ post.title }}</a>
      <span class="post-date">{{ post.date | date_to_string }} - {{ post.author }}</span>
    </li>
  </ul>
{% endfor %}