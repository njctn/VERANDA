---
layout: archive
title: "News"
permalink: /news/
author_profile: false
read_more: disabled
classes: wide
---

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign news = site.news %}
{% endif %}

{% for post in news %}
  {% include archive-single.html %}
  <p></p>
{% endfor %}
