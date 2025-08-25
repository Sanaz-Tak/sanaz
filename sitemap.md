---
layout: collection-page
title: "Sitemap"
permalink: /sitemap/
author_profile: false
---

{% include base_path %}

A clean navigation guide to all the main sections of this website. For search engines, an [XML version]({{ base_path }}/sitemap.xml) is also available.

## Main Pages
- [Home]({{ base_path }}/)
- [Portfolio]({{ base_path }}/portfolio/)
- [Publications]({{ base_path }}/publications/)
- [Teaching]({{ base_path }}/teaching/)


## Portfolio
{% for item in site.portfolio %}
  - [{{ item.title | remove: ":" }}]({{ base_path }}{{ item.url }})
{% endfor %}

## Publications
- [View all publications on Google Scholar]({{ site.author.googlescholar }})


## Teaching
{% for course in site.teaching %}
  - [{{ course.title | remove: ":" }}]({{ base_path }}{{ course.url }})
{% endfor %}
