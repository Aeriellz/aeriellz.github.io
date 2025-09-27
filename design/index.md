---
layout: page
title: the studio
---

<p>
    From having no idea how Figma works to still having no idea how Figma works. Currently still learning basic principles and getting everything wrong. But like, with style.
</p>


<p>
<h3>Projects</h3>
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