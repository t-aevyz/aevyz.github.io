---
title: First Blog Post
date: 2017-03-25 18:03:00
categories: jekyll testing
type: true
---

This is the first post for the site, just wanted to test and see if everything works out as expected.
<ul>
{% for post in site.posts %}
  {% if post.type == true%}
    <li>
    <a href="{{ site.baseurl | within: site}}{{ | within: site}}">{{ post.title | within: site }}</a><time class="pull-right post-list">{{ post.date | within: site | date_to_string | date: "%b %-d, %Y"  }}</time>
    </li>
  {% endif %}
{% endfor %}
</ul>
