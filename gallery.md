---
layout: page
title: "Distilled Insanity Gallery"
layout: default
image_folder:   /images/gallery/
sort_by:        modified_time   # modified_time or path (notice: path is case sensitive)
date_format:    "%A, %B %-d, %Y"
---

[back]({{ site.url }})


## [](#header-2) Gallery of Scotty
> Some yob that I like to make edits of their selfies

<ul class="ins-imgs">

    {% assign imgs = (site.static_files | sort: page.sort_by) %}
    {% for img in imgs reversed %}
      {% if img.path contains page.image_folder %}
        {% assign img_name = img.path | remove: page.image_folder | split: '.' | first %}
        {% assign img_date = img.modified_time | date: page.date_format %}

        <li class="ins-imgs-li" id="{{ img_name }}">
                <img src=".{{ img.path }}"
                     alt="{{ img_name }}"
                     style="max-width: {{ page.max_width }}"/>
        </li>

      {% endif %}
    {% endfor %}

</ul>

[back]({{ site.url }})
