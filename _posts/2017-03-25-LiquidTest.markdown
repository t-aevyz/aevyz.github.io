---
title: Liquid Demo For Loops
date: 2017-03-25 18:03:00
categories: jekyll testing
show: true
---


<ul>
{% for post in site.posts %}
  {% if post.show == true%}
    <li>
        <a href="{{ site.baseurl | within: site}}{{post.url | within: site}}">
          {{ post.title | within: site }}
        </a>
        <time class="pull-right post-list">
          {{ post.date | within: site | date_to_string | date: "%b %-d, %Y"  }}
        </time>

    </li>
  {% endif %}
{% endfor %}
</ul>
