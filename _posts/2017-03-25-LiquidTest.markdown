---
title: Liquid
date: 2017-03-25 18:03:00
categories: jekyll testing
type: false
---

# This is a test for Liquid Stuff
```HTML
<ul>
{% for post in site.posts %}
  {% if post.type == true%}
  <li>{{ site.baseurl }}{{ post.url }}</li>
  {% endif %}
{% endfor %}
</ul>
```
