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
      <a href="/#contact">Email</a>
    </div>
  </aside>

  <div class="home-content">
    <section id="about" class="intro-section">
      <h2>About</h2>
      <p>I am currently working as a VLA model researcher at Lumos Robotics, where I focus on robot manipulation and long-horizon tasks. My recent work includes depth-modality integration for VLA models, mask-guided object-centric manipulation, and improving non-Markovian long-horizon task execution through subtask decomposition and high-level memory modules. My research focuses on robot systems that understand physical world and generalize to open-world manipulation tasks.</p>
      <p>I am seeking PhD opportunities in robotics, especially around physical world models, VLA models, and other related areas.</p>
    </section>

    <div class="home-two-col">
      <section>
        <h2>Education</h2>
        <div class="timeline">
          <div>
            <span>2023-2025</span>
            <p><strong>MSc Robotics</strong><br>Delft University of Technology</p>
          </div>
          <div>
            <span>2019-2023</span>
            <p><strong>BEng Aircraft Design and Engineering</strong><br>Nanjing University of Aeronautics and Astronautics</p>
          </div>
        </div>
      </section>

      <section>
        <h2>Research Interests</h2>
        <ul class="compact-list">
          <li>World models for robotic manipulation</li>
          <li>Open-world object manipulation</li>
          <li>Robot planning, control, and autonomous systems</li>
        </ul>
      </section>
    </div>

    <section id="projects">
      <h2>Selected Projects</h2>
      {% assign projects = site.projects | sort: "date" | reverse %}
      <div class="publication-list project-grid">
        {% for project in projects %}
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

    <section id="experience">
      <h2>Experience</h2>
      {% assign experiences = site.experience | sort: "date" | reverse %}
      <div class="publication-list project-grid">
        {% for item in experiences %}
          <a class="publication-item" href="{{ item.url }}">
            <span>{{ item.date | date: "%Y" }}</span>
            <div>
              <h3>{{ item.title }}</h3>
              <p>{{ item.category }} · {{ item.summary }}</p>
            </div>
          </a>
        {% endfor %}
      </div>
    </section>

    <section id="contact" class="contact-section">
      <h2>Contact</h2>
      <p>
        Email: <a href="mailto:xiaotongli0105@gmail.nl">xiaotongli0105@gmail.nl</a>
        <span class="inline-separator">·</span>
        GitHub: <a href="https://github.com/Bojack-BJ" target="_blank" rel="noopener">Bojack-BJ</a>
      </p>
    </section>
  </div>
</section>
