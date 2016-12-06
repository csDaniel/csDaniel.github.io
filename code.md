---
layout: page
title: Coding Tasks
permalink: /code/
---
A list of my projects worked on while making this site:

{% for post in site.categories.code %}
  <li> <a href="{{ site.url }}{{ post.url }}"> {{ post.title }} </a>, {{ post.date | date: '%B %d, %Y' }} </li>
{% endfor %}
