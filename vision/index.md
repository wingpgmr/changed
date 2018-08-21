---
layout: default
title: "Computer Vision"
main: true
project-header: true
header-img: img/blog.jpg
description: Computer Vision
---

<ul class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.blog == true %}
{% include post-list.html %}
{% endif %}
{% endfor %}
</ul>
