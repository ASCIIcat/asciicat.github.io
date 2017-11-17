---
layout: page
title: "Distilled Insanity Gallery"
layout: default
image_folder:   /images/gallery/
max_width:      900px
sort_by:        modified_time   # modified_time or path (notice: path is case sensitive)
date_format:    "%A, %B %-d, %Y"
---


<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" type="text/css" href="style/gallerystyle.css">
</head>
<body>
[back]({{ site.url }})


## [](#header-2) Gallery of Scotty

<ul class="ins-imgs">

    {% assign imgs = (site.static_files | sort: page.sort_by) %}
    {% for img in imgs reversed %}
      {% if img.path contains page.image_folder %}
        {% assign img_name = img.path | remove: page.image_folder | split: '.' | first %}
        {% assign img_date = img.modified_time | date: page.date_format %}

        <li class="ins-imgs-li" id="{{ img_name }}">
                !["{{img_name}}"]("{{img.path}}")
        </li>

      {% endif %}
    {% endfor %}

</ul>

[back]({{ site.url }})

<footer>
    <a href="https://github.com/lthr/github-gallery" target="_blank">Powered by GitHub Gallery</a>
</footer>
