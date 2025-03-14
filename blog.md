---
layout: default
title: "Blog"
permalink: /blog/
---

# My Resume

Here’s a list of recent posts:

{% for post in site.posts %}
  <div class="post-preview">
    <a href="{{ post.url | prepend: site.baseurl }}">
      <h2>{{ post.title }}</h2>
      <p>{{ post.excerpt }}</p>
    </a>
    <p class="post-meta">Posted on {{ post.date | date: "%B %d, %Y" }}</p>
  </div>
{% endfor %}
