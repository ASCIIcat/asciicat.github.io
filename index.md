---
layout: page
title: "ASCIIcat's Dev Playground"
layout: default
description: "A place for my excess thoughts"
---
## [](#header-2) Welcome to my mind

> Here I generally rant about things.
> Though sometimes I rave about other things.


<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
