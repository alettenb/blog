---
layout: page
title: Random
---
<ul class="posts">
    {% for post in site.categories.random %}
        <li itemscope>
          <a href="{{ site.github.url }}{{ post.url }}">{{ post.title }}</a>
          <p class="post-date"><span><i class="fa fa-calendar" aria-hidden="true"></i> {{ post.date | date: "%B %-d" }} - <i class="fa fa-clock-o" aria-hidden="true"></i> {% include read-time.html %}</span></p>
        </li>
    {% endfor %}
</ul>