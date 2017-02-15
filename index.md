---
layout: page
title: "ASCIIcat's Dev Playground"
layout: default
description: "A place for my excess thoughts"
---
## [](#header-2) Welcome to my mind

> Here I generally rant about things.
> Though sometimes I rave about other things.

* * *

### [](#header-3) About Me:

<dl>
<dt>Name</dt>
<dd>Jay</dd>
<dt>Alias</dt>
<dd>ASCIIcat</dd>
<dt>Interests</dt>
<dd>Web Technology</dd>
<dd>Photography</dd>
<dd>Animé</dd>
<dd>Design</dd>
<dd>Gaming</dd>
<dt>Social</dt>
<dd>
  <ul>
    <li><a href="http://asciicatdesigns.deviantart.com/"><i class="fa fa-deviantart fa-2x" aria-hidden="true"></i></a></li>
    <li><a href="https://github.com/asciicat"><i class="fa fa-github fa-2x" aria-hidden="true"></i></a></li>
    <li><a href="https://twitter.com/ASCIIcat_Jay"><i class="fa fa-twitter fa-2x" aria-hidden="true"></i></a></li>
    <li><a href="https://www.instagram.com/asciicatdesigns/"><i class="fa fa-instagram fa-2x" aria-hidden="true"></i></a></li>
  </ul>
</dd>
</dl>

* * *

### [](#header-3) Blog:
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
