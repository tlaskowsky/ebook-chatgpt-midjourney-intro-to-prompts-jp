---
layout: default
title: Chapter 2 Subdirectory Files
---
{% assign subdirectory = "/chapter_2/" %}
<ul>
{% for file in site.static_files %}
  {% if file.path contains subdirectory %}
    <li><a href="{{ site.baseurl }}{{ file.path }}">{{ file.name }}</a></li>
  {% endif %}
{% endfor %}
</ul>

- [第２章Prompts](prompts2.md)