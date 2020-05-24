---
layout: page
title: "Distilled Insanity"
layout: default
description: "A place for my excess thoughts"
---
## [](#header-2) <span class="typer">Welcome to my mind</span>

> It is a dangerous place to be wondering around.
> Are you sure you really want to know how I tick?

Welcome to distilled_Insanity


distilled_Insanity 6.6.6 LTS


server    : 666

ip        : <span class="ipaddress"></span>

hostname  : asciicat.xyz


37 packages can be updated.

26 updates are security updates.


Last login: <span class=".datetime"></span> from <span class="ipaddress"></span>
* * *

### [](#header-3) [<span class="glitch" data-text="about_me">about_me</span>]

<dl>
<dt>Name</dt>
<dd>Jay</dd>
<dt>Alias</dt>
<dd>ASCIIcat (/ˈæskiː/-/kæt/)</dd>
<dt>Bio</dt>
<dd>I make stuff, but usually fix a lot of stuff that was never mine to begin with.</dd>
</dl>

* * *

### [](#header-3) [<span class="glitch" data-text="gallery_of_scotty">gallery_of_scotty</span>]
> Some yob that I like to make edits of their selfies

[View Gallery](./gallery)


* * *

### [](#header-3) [<span class="glitch" data-text="blog">blog</span>]
> Only the most recent posts are shown

<ul>
  {% for post in site.posts limit:3 %}
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

### [](#header-3) [<span class="glitch" data-text="social_network_stuff">social_network_stuff</span>]

<a class="tooltip" href="http://steamcommunity.com/id/ASCIIcat" data-tooltip="ASCIIcat on Steam"><i class="fa fa-steam fa-2x" aria-hidden="true"></i></a> | <a class="tooltip" href="http://asciicatdesigns.deviantart.com/" data-tooltip="ASCIIcat on deviantArt"><i class="fa fa-deviantart fa-2x" aria-hidden="true"></i></a> | <a class="tooltip" href="https://github.com/asciicat" data-tooltip="ASCIIcat on GitHub"><i class="fa fa-github fa-2x" aria-hidden="true"></i></a> | <a class="tooltip" href="https://twitter.com/ASCIIcatG" data-tooltip="ASCIIcat on Twitter"><i class="fa fa-twitter fa-2x" aria-hidden="true"></i></a> | <a class="tooltip" href="https://www.instagram.com/asciicatdesigns/" data-tooltip="ASCIIcat on Instagram"><i class="fa fa-instagram fa-2x" aria-hidden="true"></i></a> | <a class="tooltip" href="https://twitch.tv/ASCIIcat_Jay" data-tooltip="ASCIIcat on Twitch"><i class="fab fa-twitch fa-2x" aria-hidden="true"></i></a> | <a class="tooltip" href="https://asciicatdesigns.com" data-tooltip="ASCIIcatDesigns Photography & Design"><i class="fas fa-camera-retro fa-2x" aria-hidden="true"></i></a>
