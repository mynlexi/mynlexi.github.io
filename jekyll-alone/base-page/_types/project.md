---
short_name: project
name: My Projects
---
Here are all my projects

<ul>
  {% assign filtered_posts = site.posts | where: 'type', page.short_name %}
  {% for post in filtered_posts %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>