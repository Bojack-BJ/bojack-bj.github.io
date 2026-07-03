---
layout: default
title: Home
description: Robotics researcher working on open-world manipulation, world models, and robot autonomy.
---

<section class="home-grid">
  <aside class="profile-panel">
    <img class="portrait" src="/images/avatar.jpg" alt="Portrait of Xiaotong Li">
    <h1>Xiaotong Li</h1>
    <p>Robotics researcher interested in world models, open-world manipulation, and autonomous robot systems.</p>
    <div class="profile-links">
      <a href="/uploads/cv.pdf">CV</a>
      <a href="https://github.com/Bojack-BJ" target="_blank" rel="noopener">GitHub</a>
      <a href="/contact/">Email</a>
    </div>
  </aside>

  <div class="home-content">
    <section class="intro-section">
      <h2>About</h2>
      <p>I am completing my MSc in Robotics at Delft University of Technology. My research focuses on robot systems that understand object dynamics, reason about physical interaction, and generalize to open-world manipulation tasks.</p>
      <p>I am seeking PhD opportunities in robotics, especially around world models, open-world manipulation, and embodied autonomy.</p>
    </section>

    <section>
      <h2>Research Interests</h2>
      <ul class="compact-list">
        <li>World models for robotic manipulation</li>
        <li>Open-world object manipulation</li>
        <li>Robot planning, control, and autonomous systems</li>
      </ul>
    </section>

    <section>
      <h2>Education</h2>
      <div class="timeline">
        <div>
          <span>2023-2025</span>
          <p><strong>MSc Robotics</strong>, Delft University of Technology</p>
        </div>
        <div>
          <span>2019-2023</span>
          <p><strong>BEng Aircraft Design and Engineering</strong>, Nanjing University of Aeronautics and Astronautics</p>
        </div>
      </div>
    </section>

    <section>
      <h2>Selected Projects</h2>
      {% assign projects = site.projects | sort: "date" | reverse %}
      <div class="publication-list">
        {% for project in projects limit: 4 %}
          <a class="publication-item" href="{{ project.url }}">
            <span>{{ project.date | date: "%Y" }}</span>
            <div>
              <h3>{{ project.title }}</h3>
              <p>{{ project.summary }}</p>
            </div>
          </a>
        {% endfor %}
      </div>
    </section>
  </div>
</section>
