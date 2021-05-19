---
layout: default
title: Home
---

# Welcome to Ricardo's notes #

I use this online garden as a place to register my ideas and expose them to my friends and to whoever might be interested. Most articles are works in progress. Feel free to make any suggestions or even pull requests for anything you may like.

<h2>Latest Posts</h2>

<ul>
  {% for post in site.posts %}
    <li>
      <h4>{% if post.completedness %}({{ post.completedness}}){% endif %} <a href="{{ post.url }}">{{ post.title }}</a></h4> 
      <!-- {{ post.excerpt }} -->
    </li>
  {% endfor %}
</ul>
