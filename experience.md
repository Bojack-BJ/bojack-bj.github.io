---
layout: page
title: Experience
permalink: /experience/
summary: Internships, engineering work, and robotics competitions.
---

{% assign experiences = site.experience | sort: "date" | reverse %}
<div class="card-list">
{% for item in experiences %}
  <a class="list-card" href="{{ item.url }}">
    <span>{{ item.date | date: "%Y" }} · {{ item.category }}</span>
    <h2>{{ item.title }}</h2>
    <p>{{ item.summary }}</p>
  </a>
{% endfor %}
</div>
