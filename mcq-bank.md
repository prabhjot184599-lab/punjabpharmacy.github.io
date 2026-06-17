---
layout: page
title: MCQ Bank
permalink: /mcq-bank/
---

Practice daily high-yield Pharmacy MCQs for rapid revision.

<ul>
  {% assign filtered_posts = site.posts | where: "categories", "mcqs" %}
  {% for post in filtered_posts %}
    <li>
      <strong>{{ post.date | date: "%b %d, %Y" }}</strong> &raquo; 
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% else %}
    <li>No MCQs posted yet. Check back soon!</li>
  {% endfor %}
</ul>
