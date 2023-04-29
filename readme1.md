---
layout: default
title: Chapter 1 Subdirectory Files
---
{% assign subdirectory = "/chapter_1/" %}
<ul>
{% for file in site.static_files %}
  {% if file.path contains subdirectory %}
    <li><a href="{{ site.baseurl }}{{ file.path }}">{{ file.name }}</a></li>
  {% endif %}
{% endfor %}
</ul>