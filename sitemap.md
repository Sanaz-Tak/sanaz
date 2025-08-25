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
{% for pub in site.publications %}
  - [{{ pub.title }}]({{ base_path }}{{ pub.url }}) - {{ pub.date | date: "%Y" }}
{% endfor %}

## Portfolio
{% for item in site.portfolio %}
  - [{{ item.title | remove: ":" }}]({{ base_path }}{{ item.url }})
{% endfor %}

## Teaching
{% for course in site.teaching %}
  - [{{ course.title | remove: ":" }}]({{ base_path }}{{ course.url }})
{% endfor %}
