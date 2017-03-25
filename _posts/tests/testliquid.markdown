---
title: Liquid Demo For Loops
date: 2017-03-25 18:03:00
categories: Site_Tests
show: false
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

<a href="{{site.baseurl}}LiquidTestDemo.html">Hyperlink To Hidden Page</a>
