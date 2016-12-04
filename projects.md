---
layout: page
title: Projects
permalink: /project/
---
A list of my projects worked on while making this site:

{% for post in site.categories.project %}
  <li> <a href="{{ site.url }}{{ post.url }}"> {{ post.title }} </a>, {{ post.date | date: '%B %d, %Y' }} </li>
{% endfor %}
