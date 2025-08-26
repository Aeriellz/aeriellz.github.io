---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

*Hello!*

My name is Ariel (she/her), and you just found my blog!

This is a space in constant and permanent construction. It is a home for my thoughts and creations as I develop a myriad of hobbies and interests.

Thanks so much for dropping by!


Here's the categories:

{% for category in site.categories %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}