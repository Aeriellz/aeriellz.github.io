---
layout: page
title: on design
---

All posts and projects related to graphical design, from mixed media to complaining about photoshop.

#### All posts
{% for post in  site.categories.design %}
{{ post.title }} {{ post.date | date: "%m-%d-%Y" }}
{% endfor %}

