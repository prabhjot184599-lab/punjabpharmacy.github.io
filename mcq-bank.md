
---
layout: page
title: MCQ Bank
permalink: /mcq-bank/
---

Practice daily high-yield Pharmacy MCQs for rapid revision.

<ul>
  {% for post in site.categories.mcqs %}
    <li>
      <strong>{{ post.date | date: "%b %d, %Y" }}</strong> &raquo; 
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% else %}
    <li>No MCQs posted yet. Check back soon!</li>
  {% endfor %}
</ul>
