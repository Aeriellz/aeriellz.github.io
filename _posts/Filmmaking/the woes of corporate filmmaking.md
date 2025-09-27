

complain about not being able to post the cool shit i made because my contract says i can't do it and i don't wanna be sued out of money i don't have




---

layout: page

title: the skyline view workshop

---

  

<p>

From breadboards to webstack explorations. Currently, I'm taking CS50 and learning the basics of the discipline.

</p>

  
  

<p>

<h3>Projects</h3>

</p>

  
  

<p>

<h3>All posts</h3>

</p>

<section class="posts">

<ul>

{% for post in site.categories.compsci %}

<li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a><time

datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%m-%d-%Y" }}</time></li>

{% endfor %}

</ul>

</section>