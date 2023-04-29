---
layout: default
title: Chapter 5 Subdirectory Files
---
{% assign subdirectory = "/chapter 5/" %}
<ul>
{% for file in site.static_files %}
  {% if file.path contains subdirectory %}
    <li><a href="{{ site.baseurl }}{{ file.path }}">{{ file.name }}</a></li>
  {% endif %}
{% endfor %}
</ul>