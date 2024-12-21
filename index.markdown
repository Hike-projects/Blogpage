---
layout: default
title: Blogposts
---
# Blogposts

Welcome to my blog! Below are the latest posts:

<ul>
    {% for post in site.posts %}
    <li>
        <a href="{{ post.url }}">{{ post.title }}</a>  
        <small>{{ post.date | date: "%B %d, %Y" }}</small>
    </li>
    {% endfor %}
</ul>
