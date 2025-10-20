---
layout: page
title: the studio on mulholland drive
---
<p>
<i>Nuthouse California Studios is a deceptively modest construction tucked between the curves of Mullholand Dr., woven in between the trees, overlooking LA. You walk in to a very californian work environment: futons, people sprawled on couches, whiteboards in the middle of the room. The sound stage is in the back, the receptionist said. Editing to the left, screening is downstairs. The writers commandeered the conference floor years ago for some project or another and refused to leave, so you'll find them all there.</i>
<p>
<i>In her wildest dreams, the owner would have the place built inside Redwood National Park, but not only that's illegal, that would be, according to herself, "ecologically immoral". So she settled for Mullholand, which sounded to her wife as completely unhinged—whenever the hell has anyone "settled" for Mullholand Drive?
</i>
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