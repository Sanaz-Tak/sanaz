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
- [Teaching]({{ base_path }}/teaching/)
- [Publications]({{ base_path }}/publications/)


## Publications
- [View all publications on Google Scholar]({{ site.author.googlescholar }})

*Note: For a complete list of publications, visit my [Google Scholar profile]({{ site.author.googlescholar }}).*

## Portfolio
{% for item in site.portfolio %}
  - [{{ item.title | remove: ":" }}]({{ base_path }}{{ item.url }})
{% endfor %}

## Teaching
{% for course in site.teaching %}
  - [{{ course.title | remove: ":" }}]({{ base_path }}{{ course.url }})
{% endfor %}
