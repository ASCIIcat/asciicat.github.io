---
layout: page
title: "ASCIIcat's Dev Playground"
layout: default
description: "A place for my excess thoughts"
---
[back]({{ site.url }})


## [](#header-2) All Blog Posts

> Here are all my posts, untill I figure out how to do propper pagination
> Since Jekyll has depreicated it and I am not able to load custom plugins
> on Github Pages...

* * *

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <p class="post-excerpt">

        {% if post.content contains '<!--excerpt.start-->' and post.content contains '<!--excerpt.end-->' %}
        	> {{ ((post.content | split:'<!--excerpt.start-->' | last) | split: '<!--excerpt.end-->' | first) | strip_html | truncatewords: 20 }}

        {% else %}
        	> {{ post.content | strip_html | truncatewords: 20 }}

        {% endif %}

      </p>
    </li>
  {% endfor %}
</ul>

[back]({{ site.url }})
