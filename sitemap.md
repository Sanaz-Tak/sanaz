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
- [About]({{ base_path }}/)
- [CV]({{ base_path }}/cv/)
- [Portfolio]({{ base_path }}/portfolio/)
- [Teaching]({{ base_path }}/teaching/)
- [Publications]({{ base_path }}/publications/)
- [Talks]({{ base_path }}/talks/)

## Blog Posts
{% for post in site.posts limit:10 %}
  - [{{ post.title }}]({{ base_path }}{{ post.url }}) - {{ post.date | date: "%B %Y" }}
{% endfor %}
{% if site.posts.size > 10 %}
  - *... and [{{ site.posts.size | minus: 10 }} more posts](/posts/)*
{% endif %}

## Publications
{% for pub in site.publications %}
  - [{{ pub.title }}]({{ base_path }}{{ pub.url }}) - {{ pub.date | date: "%Y" }}
{% endfor %}

## Portfolio
{% for item in site.portfolio %}
  - [{{ item.title }}]({{ base_path }}{{ item.url }})
{% endfor %}

## Teaching
{% for course in site.teaching %}
  - [{{ course.title }}]({{ base_path }}{{ course.url }})
{% endfor %}

## Talks
{% for talk in site.talks %}
  - [{{ talk.title }}]({{ base_path }}{{ talk.url }}) - {{ talk.date | date: "%B %Y" }}
{% endfor %}
