---
title: HTML Attempt
date: 2017-03-25 18:03:00
categories: jekyll testing
type: false
---

# This is a test for type notBlog v1
<ul>
{% for post in site.posts %}

  <li>
  <a href="
  {{ site.baseurl }}{{ post.url }}
  ">URL</a>
  </li>
{% endfor %}
</ul>
