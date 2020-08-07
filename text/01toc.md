---
title: Contents 
chapter: ii.
frontmatter: true
---

<hr>

<h1 class="toc-title">CONTENTS</h1>

{%- assign chapters = site.html_pages | where: "layout", "chapter" -%}
{%- assign parts = chapters | where_exp: "c","c.part-title != null" -%}

{% for p in parts %}
<h2>{{ p.part-title }}</h2>
{% assign items = chapters | where: "part", p.part %}
<ol class="toc-list">
  {% for i in items %}
  <li><a href="{{ i.url | absolute_url }}">{{ i.title }}</a></li>
  {% endfor %}
</ol>
{% endfor %}
<hr>
