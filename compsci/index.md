---
layout: page
title: the skyline view workshop
---
<p>
    From breadboards to webstack explorations. Currently, I'm taking CS50 and learning the basics of the discipline.
</p>


<section class="posts">
<p>
<h3>Projects</h3>
</p>

<p>
<h3>All posts</h3>
</p>
    <ul>
        {% for post in site.categories.compsci %}
        <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a><time
                datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%m-%d-%Y" }}</time></li>
        {% endfor %}
    </ul>
</section>