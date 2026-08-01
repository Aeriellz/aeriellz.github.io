---
layout: default
lang: eng
---

<section class="posts">

<b>Frame</b> <i>/frām/
<br>Noun.</i>
An open case or structure made for admitting, enclosing, or supporting something.
</p>
<br>
<br>
{% assign posts=site.posts | where:"lang", page.lang %}
<ul>
{% for post in posts %}
        <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a><time
         datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%m-%d-%Y" }}</time></li>
{% endfor %}
</ul>
</section>


