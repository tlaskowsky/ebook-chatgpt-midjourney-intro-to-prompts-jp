---
layout: default
title: Chapter 3 Subdirectory Files
---
{% assign subdirectory = "/chapter_3/" %}
<ul>
{% for file in site.static_files %}
  {% if file.path contains subdirectory %}
    <li><a href="{{ site.baseurl }}{{ file.path }}">{{ file.name }}</a></li>
  {% endif %}
{% endfor %}
</ul>

- [第３章Prompts](prompts3.md)