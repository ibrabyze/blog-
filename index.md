---
layout: default
title: "SEO Content Engine OS™ Blog"
---

<h1>Latest Articles</h1>

<ul class="post-list">
  {% for post in site.posts %}
    <li class="post-item">
      <div class="post-date">{{ post.date | date: "%B %d, %Y" }}</div>
      <h3>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
      {% if post.description %}
        <div class="post-excerpt">
          {{ post.description }}
        </div>
      {% endif %}
    </li>
  {% endfor %}
</ul>
