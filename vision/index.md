---
layout: default
title: "Computer Vision"
main: true
project-header: true
header-img: img/about.jpg
description: Computer Vision 에 관하여 글을 올립니다.
---

<ul class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.blog == true %}
{% include post-list.html %}
{% endif %}
{% endfor %}
</ul>
