---
layout: default
title: "Home"
---

## Latest Posts

{% for post in site.posts %}
  <article>
    <header>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p>{{ post.date | date: "%B %d, %Y" }}</p>
    </header>

    <div class="excerpt">
      {{ post.excerpt }} <!-- Excerpt of the post -->
      <a href="{{ post.url | relative_url }}">Read More</a> <!-- This links to the full post -->
    </div>
  </article>
{% endfor %}
