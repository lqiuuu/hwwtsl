---
layout: archive
lang: en
title: "Letter Collection"
which_category: letter
permalink: /correspondence/
---
{% assign current_lang = page.lang | default: 'en' %}
<ul>
  {% for post in site.posts %}
    {% if post.lang == current_lang %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>