---
layout: default
---

<section class="posts">
<h1>Tag #Homelab</h1>
    <ul>
      {% for post in site.tags.homelab %}
      <li><a class="post" href="{{ post.url }}">{{ post.title }}</a><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%m-%d-%Y" }}</time></li>
      {% endfor %}
    </ul>
    
</section>