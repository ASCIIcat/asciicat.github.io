---
layout: page
title: "Distilled Insanity"
layout: default
description: "A place for my excess thoughts"
---
## [](#header-2) <span class="typer">Welcome to my mind</span>

> Here I generally rant about things.
> Though sometimes I rave about other things.

* * *

### [](#header-3) [about_me]

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
<dd>日本</dd>
</dl>

* * *

### [](#header-3) [gallery_of_scotty]
> Some yob that I like to make edits of their selfies

[View Gallery](./gallery)


* * *

### [](#header-3) [blog]
> Only the most recent posts are shown

<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url }}">{{ post.date | date: "%F" }} - {{ post.title }}</a>
      <p class="post-excerpt">

        {% if post.content contains '<!--excerpt.start-->' and post.content contains '<!--excerpt.end-->' %}
        	 {{ ((post.content | split:'<!--excerpt.start-->' | last) | split: '<!--excerpt.end-->' | first) | strip_html | truncatewords: 20 }}
        {% else %}
        	 {{ post.content | strip_html | truncatewords: 20 }}
        {% endif %}

      </p>
    </li>
  {% endfor %}
</ul>

[All posts](./allposts)

* * *

### [](#header-3) [social_network_stuff]

<a class="tooltip" href="http://steamcommunity.com/id/ASCIIcat" data-tooltip="ASCIIcat on Steam"><i class="fa fa-steam fa-2x" aria-hidden="true"></i></a> | <a class="tooltip" href="http://asciicatdesigns.deviantart.com/" data-tooltip="ASCIIcat on deviantArt"><i class="fa fa-deviantart fa-2x" aria-hidden="true"></i></a> | <a class="tooltip" href="https://github.com/asciicat" data-tooltip="ASCIIcat on GitHub"><i class="fa fa-github fa-2x" aria-hidden="true"></i></a> | <a class="tooltip" href="https://twitter.com/ASCIIcat_Jay" data-tooltip="ASCIIcat on Twitter"><i class="fa fa-twitter fa-2x" aria-hidden="true"></i></a> | <a class="tooltip" href="https://www.instagram.com/asciicatdesigns/" data-tooltip="ASCIIcat on Instagram"><i class="fa fa-instagram fa-2x" aria-hidden="true"></i></a> | <a class="tooltip" href="https://player.me/asciicat" data-tooltip="ASCIIcat on Player.Me"><img src="https://player.me/logo-250-2.png" style="width: 27px;" /></a>
