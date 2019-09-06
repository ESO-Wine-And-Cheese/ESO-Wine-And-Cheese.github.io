---
layout: layout
title: "Posts"
---


<section class="content">

Previous Wine & Cheese seminars
===============

<ul class="listing">
  {% assign past_posts = (site.posts | where: "category" , "past") %}
  {% for post in past_posts %}
  <li>
  <span>{{ post.date | date: "%B %e, %Y" }}</span> <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
  </li>
  {% endfor %}
</ul>
</section>
