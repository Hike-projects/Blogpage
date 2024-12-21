---
layout: default
title: Home
---
<div class="homepage">
    <h1>Welcome to My Blog</h1>
    <p>This is the homepage of my Jekyll site!</p>
    <ul>
        {% for post in site.posts %}
        <li>
            <a href="{{ post.url }}">{{ post.title }}</a>
            <small>{{ post.date | date: "%B %d, %Y" }}</small>
        </li>
        {% endfor %}
    </ul>
</div>
