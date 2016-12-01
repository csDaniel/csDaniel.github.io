---
layout: page
title: Stories
permalink: /story/
---
A list of my postings related to my thought process while working on a project or this site:

{% for post in site.categories.story %}
  <li> <a href="{{ site.url }}{{ post.url }}"> {{ post.title }} </a>, {{ post.date | date: '%B %d, %Y' }} </li>
{% endfor %}
