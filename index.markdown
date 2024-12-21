---
layout: default
title: Home
---
# Welcome to My Blog

This is the homepage of my Jekyll site.

Here are my blog posts:

<ul>
    {% for post in site.posts %}
    <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        <small>{{ post.date | date: "%B %d, %Y" }}</small>
    </li>
    {% endfor %}
</ul>
