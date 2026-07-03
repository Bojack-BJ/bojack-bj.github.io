---
layout: page
title: Projects
permalink: /projects/
summary: Research and engineering projects across robot manipulation, planning, control, and autonomous systems.
---

{% assign projects = site.projects | sort: "date" | reverse %}
<div class="card-list">
{% for project in projects %}
  <a class="list-card" href="{{ project.url }}">
    <span>{{ project.date | date: "%B %Y" }}</span>
    <h2>{{ project.title }}</h2>
    <p>{{ project.summary }}</p>
  </a>
{% endfor %}
</div>
