---
title: Liquid
date: 2017-03-25 18:03:00
categories: jekyll testing
type: false
---

# This is a test for Liquid Stuff

{% for post in site.posts %}
  {% if post.type == true%}
  {{ site.baseurl }}{{ post.url }}
  {% endif %}
{% endfor %}
