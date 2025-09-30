---
layout: page
title: the writers room floor
---
<p>
    From screenwriting commentary to film stock experiments. Currently extremely tired of this bullshit after two failed attempts at getting a Fulbright scholarship.
</p>

{% include collapsibleFilmmaking.html %}

<section class="posts">
<p>
<h3>All posts</h3>
</p>
    <ul>
        {% for post in site.categories.filmmaking %}
        <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a><time
                datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%m-%d-%Y" }}</time></li>
        {% endfor %}
    </ul>
</section>