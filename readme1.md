---
layout: default
title: Chapter 1 Files
---
{% assign subdirectory = "/chapter_1/" %}
<ul>
{% for file in site.static_files %}
  {% if file.path contains subdirectory %}
    <li><a href="{{ site.baseurl }}{{ file.path }}">{{ file.name }}</a></li>
  {% endif %}
{% endfor %}
</ul>

1. [第１章Prompts](prompts1.md)