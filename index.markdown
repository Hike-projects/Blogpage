---
layout: default
title: "Home"
---

## Latest Posts

{% for post in site.posts %}
  <article>
    <header>
      <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.date | date: "%B %d, %Y" }}</p>
    </header>

    <div class="excerpt">
      {{ post.excerpt }}
      <a href="{{ site.baseurl }}{{ post.url }}">Read More</a>
    </div>
  </article>
{% endfor %}
