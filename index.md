---
layout: default
title: Home
description: Robotics researcher working on open-world manipulation, world models, and robot autonomy.
---

<section class="hero">
  <div class="hero-copy">
    <p class="eyebrow">Robotics · World Models · Open-World Manipulation</p>
    <h1>Xiaotong Li</h1>
    <p class="hero-text">I am a robotics researcher interested in building robot systems that understand object dynamics, reason about physical interaction, and generalize to open-world manipulation tasks.</p>
    <div class="hero-actions">
      <a class="button primary" href="/projects/">View research projects</a>
      <a class="button" href="/uploads/cv.pdf">Download CV</a>
      <a class="button" href="https://github.com/Bojack-BJ" target="_blank" rel="noopener">GitHub</a>
    </div>
  </div>
  <img class="portrait" src="/images/avatar.jpg" alt="Portrait of Xiaotong Li">
</section>

<section class="section-grid">
  <div>
    <p class="eyebrow">Current Focus</p>
    <h2>Explicit world models for robotic manipulation</h2>
    <p>I recently worked on open-world object manipulation without task-specific action demonstrations, combining open-set perception, digital twin reconstruction, and simulation-based strategy sampling.</p>
  </div>
  <div class="fact-list">
    <div>
      <strong>MSc Robotics</strong>
      <span>Delft University of Technology, 2023-2025</span>
    </div>
    <div>
      <strong>BEng Aircraft Design and Engineering</strong>
      <span>Nanjing University of Aeronautics and Astronautics, 2019-2023</span>
    </div>
    <div>
      <strong>Research Interests</strong>
      <span>World models, open-world manipulation, robot planning, autonomous systems</span>
    </div>
  </div>
</section>

<section class="listing">
  <div class="section-title">
    <p class="eyebrow">Selected Work</p>
    <h2>Projects</h2>
  </div>
  {% assign projects = site.projects | sort: "date" | reverse %}
  {% for project in projects limit: 3 %}
    <a class="list-card" href="{{ project.url }}">
      <span>{{ project.date | date: "%Y" }}</span>
      <h3>{{ project.title }}</h3>
      <p>{{ project.summary }}</p>
    </a>
  {% endfor %}
</section>
