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
      <p>I am currently working as a VLA model researcher at Lumos Robotics, where I focus on robot manipulation and long-horizon tasks. My recent work includes depth-modality integration for VLA models, mask-guided object-centric manipulation, and improving non-Markovian long-horizon task execution through subtask decomposition and high-level memory modules. More broadly, I am interested in physical world models, open-world manipulation, and robot learning that can understand and interact with the physical world.</p>
      <p>I am seeking PhD opportunities in robotics, especially around physical world models, VLA models, and other related areas.</p>
    </section>

    <section class="education-section">
      <h2>Education</h2>
      <div class="timeline education-list">
        <div>
          <span>2023-2025</span>
          <p><strong>MSc Robotics, Delft University of Technology</strong></p>
        </div>
        <div>
          <span>2019-2023</span>
          <p><strong>BEng Aircraft Design and Engineering, Nanjing University of Aeronautics and Astronautics</strong></p>
        </div>
        <div>
          <span>2022 Jul</span>
          <p><strong>Robotics Summer School, Korea Advanced Institute of Science & Technology (KAIST)</strong></p>
        </div>
      </div>
    </section>

    <section id="projects">
      <h2>Selected Projects</h2>
      {% assign projects = site.projects | sort: "date" | reverse %}
      <div class="project-list">
        {% for project in projects %}
          <article class="project-item">
            <a class="project-thumb" href="{{ project.url }}" aria-label="{{ project.title }}">
              {% if project.thumbnail %}
                <img src="{{ project.thumbnail }}" alt="">
              {% else %}
                <span>{{ project.date | date: "%Y" }}</span>
              {% endif %}
            </a>
            <div class="project-body">
              <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
              <p class="project-meta-line">{{ project.date | date: "%Y" }}{% if project.tags %} · {{ project.tags | join: " / " }}{% endif %}</p>
              <p>{{ project.summary }}</p>
              <div class="project-link-row">
                <a href="{{ project.url }}">Project</a>
                {% for link in project.links %}
                  <a href="{{ link.url }}" target="_blank" rel="noopener">{{ link.label }}</a>
                {% endfor %}
              </div>
            </div>
          </article>
        {% endfor %}
      </div>
    </section>

    <section id="experience">
      <h2>Internships</h2>
      <div class="timeline experience-list">
        <div>
          <span>2025-now</span>
          <p><strong>Embodied AI Engineer</strong>, Lumos Robotics, Suzhou<br>Designed data collection pipelines based on FastUMI and developed VLA algorithms for real-robot manipulation and long-horizon tasks.</p>
        </div>
        <div>
          <span>2024</span>
          <p><strong>Research Intern</strong>, TU Delft Autonomous Multi-Robots Lab, Delft<br>Worked on real-time point cloud completion for robots using Transformer-based completion and category-level object pose estimation.</p>
        </div>
        <div>
          <span>2023</span>
          <p><strong>ROS Engineer</strong>, Bayer Crop Science, Shanghai<br>Built an Isaac Sim digital twin platform for agricultural robot algorithm iteration.</p>
        </div>
      </div>
    </section>

    <section id="awards">
      <h2>Awards</h2>
      <div class="award-grid">
        <div>
          <h3>Competitions</h3>
          <ul class="compact-list">
            <li>RoboMaster 2021 National, third prize</li>
            <li>RoboMaster 2021 Central Division, second prize</li>
            <li>RoboCup China Open 3D Detection, third prize</li>
            <li>RoboCup China Open Medical Robots Track, third prize</li>
            <li>Jiangsu Provincial Engineering Training Competition, second prize</li>
            <li>RoboMaster 2020 Online, second prize</li>
          </ul>
        </div>
        <div>
          <h3>Academic Honors</h3>
          <ul class="compact-list">
            <li>First-Class Academic Scholarship, 3 times</li>
            <li>Second-Class Excellent Student Scholarship, 2 times</li>
            <li>Merit Student Honor, 2 times</li>
          </ul>
        </div>
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
