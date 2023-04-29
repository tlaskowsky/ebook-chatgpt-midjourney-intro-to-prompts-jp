### 「ChatGPT＋Midjourneyでデジタルアートを極める！英語プロンプト術入門」のリソース集

1. [第１章リソース](/chapter 1/readme.md)
1. [第２章リソース](/chapter 2/readme.md)
1. [第３章リソース](/chapter 3/readme.md)
1. [第４章リソース](/chapter 4/readme.md)
1. [第５章リソース](/chapter 5/readme.md)
1. [第６章リソース](/chapter 6/readme.md)


{% assign subdirectory = "chapter 1" %}
<ul>
{% for chapter in site.chapters %}
  {% assign chapter_parent_directory = chapter.path | split: '/' | first %}
  {% if chapter_parent_directory == subdirectory %}
    <li><a href="{{ site.baseurl }}{{ chapter.url }}">{{ chapter.title | default: chapter.name }}</a></li>
  {% endif %}
{% endfor %}
</ul>