---
title: Home
layout: template
filename: index.md
--- 

# AlexanderTsuetaki.github.io
My_Website a persional project
Jekly theme used: Slate

<div class="post-list">
    {% for post in site.posts %}
    
        <a class="post-title" href="{{site.baseurl}}{{post.url}}"><h2>{{ post.title }}</h2></a>
        <p class="date">{{ post.date | date: "%b %-d, %Y" }}</p>
        <p>{{post.excerpt | strip_html}}</p>
    
    {% endfor %}
</div>