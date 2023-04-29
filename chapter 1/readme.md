---
layout: default
title: Chapter 1 Subdirectory Files
---

{% assign subdirectory = "/chapter 1/" %}
{% assign exclude_subdirectory = "/chapter 1/images/" %}
<ul>
{% for file in site.static_files %}
  {% if file.path contains subdirectory and file.path contains exclude_subdirectory %}
    {% continue %}
  {% elsif file.path contains subdirectory %}
    <li><a href="{{ site.baseurl }}{{ file.path }}">{{ file.name }}</a></li>
  {% endif %}
{% endfor %}
</ul>

