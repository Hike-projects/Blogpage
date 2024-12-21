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
      {{ post.excerpt }}  <!-- This will display the post excerpt (content before <!--more--> tag) -->
      <a href="{{ post.url | relative_url }}">Read More</a>  <!-- "Read More" link to full post -->
    </div>
  </article>
{% endfor %}
