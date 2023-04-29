---
layout: default
title: Chapter 2 Subdirectory Files
---
{% assign subdirectory = "/chapter 2/" %}
<ul>
{% for file in site.static_files %}
  {% if file.path contains subdirectory %}
    <li><a href="{{ file.path }}">{{ file.name }}</a></li>
  {% endif %}
{% endfor %}
</ul>