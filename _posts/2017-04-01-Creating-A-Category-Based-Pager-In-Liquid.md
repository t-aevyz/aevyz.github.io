---
title: Creating a Category Based Pager in Liquid for Jekyll
date: 2017-04-01 01:26
categories: adv-jekyll
series:  Advanced Customization of Jekyll

---

For those that are impatient, here is the code that I used:
<div id="spoiler" style="display:none">
<code>
&#123;% assign prev = "" %&#125;<br>
&#123;% assign next = "" %&#125;<br>
&#123;% assign stop = false %&#125;<br>

&#123;% for post in site.posts%&#125;<br>
  &#123;% if post == page %&#125;<br>
    &#123;% assign stop = true %&#125;<br>
  &#123;% elsif post.categories == page.categories %&#125;<br>
    &#123;% if stop %&#125;<br>
        &#123;% assign prev = post.url %&#125;<br>
        &#123;% assign pTitle = post.title %&#125;<br>
        &#123;% break %&#125;<br>
    &#123;% else %&#125;<br>
        &#123;% assign next = post.url %&#125;<br>
        &#123;% assign nTitle = post.title %&#125;<br>
    &#123;% endif %&#125;<br>
  &#123;% endif %&#125;<br>

&#123;% endfor%&#125;<br>

&#123;% if prev != "" %&#125;<br>
  &lt;li class="previous"&gt;&lt;a href="&#123;&#123; prev &#125;&#125;"&gt;&larr; Previous Page  -  &#123;&#123;pTitle&#125;&#125;&lt;/a&gt;&lt;/li&gt;<br>
&#123;% endif %&#125;<br>
&#123;% if next != "" %&#125;<br>
    &lt;li class="next"&gt;&lt;a href="&#123;&#123; next &#125;&#125;"&gt; Next Page  -  &#123;&#123;nTitle&#125;&#125; &rarr;&lt;/a&gt;&lt;/li&gt;<br>
&#123;% endif %&#125;<br>

</code>
</div>
<button title="Click to show/hide code" type="button" onclick="if(document.getElementById('spoiler') .style.display=='none') {document.getElementById('spoiler') .style.display=''}else{document.getElementById('spoiler') .style.display='none'}">Show/Hide Code</button>
