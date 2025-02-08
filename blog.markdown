---
layout: default
title: Blog Posts
permalink: /blog/
description: Read my latest blog posts and articles
---

# Blog Posts

{% for post in site.posts %}
  <article class="post-preview">
    <h2>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h2>
    <p class="post-meta">Posted on {{ post.date | date: "%B %d, %Y" }}</p>
    {% if post.description %}
      <p>{{ post.description }}</p>
    {% endif %}
  </article>
  <hr>
{% endfor %}

[Back to Home](/portfolio/) 