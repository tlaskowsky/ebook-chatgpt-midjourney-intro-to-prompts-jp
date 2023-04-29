---
layout: default
title: Chapter 1 Subdirectory Files
---

{% assign subdirectory = "{{ site.baseurl }}chapter 1/" %}
{% assign exclude_subdirectory = "{{ site.baseurl }}images/" %}
<ul>
{% for file in site.static_files %}
  {% if file.path contains subdirectory and file.path contains exclude_subdirectory %}
    {% continue %}
  {% elsif file.path contains subdirectory %}
    <li><a href="{{ site.baseurl }}{{ file.path }}">{{ file.name }}</a></li>
  {% endif %}
{% endfor %}
</ul>

