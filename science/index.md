---
layout: page
title: the empty amphitheater
---

<p>
    From economics to physics. Currently remembering what is like to love what I love.
</p>

<p>
<h3>All posts</h3>
</p>
<section class="posts">
    <ul>
        {% for post in site.categories.design %}
        <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a><time
                datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%m-%d-%Y" }}</time></li>
        {% endfor %}
    </ul>
</section>