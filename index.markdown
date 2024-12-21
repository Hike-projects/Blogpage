---
layout: default
title: Home
---

<h2>Latest Blog Posts</h2>

{% for post in site.posts %}
  <article>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="date">{{ post.date | date: "%B %d, %Y" }}</p>
    
    <!-- Displaying the post excerpt or truncated content -->
    {% if post.excerpt %}
      <p>{{ post.excerpt }}</p>
    {% else %}
      <p>{{ post.content | strip_html | truncatewords: 40 }}</p> <!-- Show first 40 words -->
    {% endif %}
    
    <a href="{{ post.url | relative_url }}">Read more</a>
  </article>
{% endfor %}
