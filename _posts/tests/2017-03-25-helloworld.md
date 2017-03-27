---
title: Hello World
date: 2017-03-25 00:00:00
categories: General
show: false
---

## Hello World

This is going to be my first "proper" post using Jekyll and I am going to be seeing how this functions.


This is going to be a test for liquid stuff:

{% for post in site.posts %}
#BEGIN FOR LOOP:



  {% assign words = post.content | split: '<br>' %}

  {% for word in words limit:1 %}
    {{ word }}
  {% endfor %}
#END FOR LOOP


{% endfor %}
