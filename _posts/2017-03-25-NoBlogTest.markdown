---
title: HTML Attempt
date: 2017-03-25 18:03:00
categories: jekyll testing
type: false
---

# This is a test for type notBlog
<ul>
{% for post in site.posts %}
  {% if post.type == true%}
  <li><a href="{{ site.baseurl }}{{ post.url }}">URL</a></li>
  {% endif %}
{% endfor %}
</ul>
