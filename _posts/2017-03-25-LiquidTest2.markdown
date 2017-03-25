---
title: LiquidTesting2
date: 2017-03-25 18:03:00
categories: jekyll testing
type: true
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
