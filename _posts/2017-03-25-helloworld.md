---
title: Hello World
date: 2017-03-25 18:03:00
categories: General
show: true
---

## Hello World

This is going to be my first "proper" post using Jekyll and I am going to be seeing how this functions.


This is going to be a test for liquid stuff:

{% for post in site.posts %}

  {% assign words = post.content | split: '\n' %}

  {% for word in words limit:2 %}
    {{ word }}
  {% endfor %}
NEXT LINE
{% endfor %}
