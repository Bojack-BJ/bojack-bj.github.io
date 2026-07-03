---
layout: default
title: Home
description: Robotics researcher working on open-world manipulation, world models, and robot autonomy.
---

<section class="home-grid">
  <aside class="profile-panel">
    <img class="portrait" src="/images/avatar.jpg" alt="Portrait of Xiaotong Li">
    <h1>Xiaotong Li</h1>
    <p>Robotics researcher interested in world models, VLA models, and robot learning.</p>
    <div class="profile-links">
      <a class="profile-link" href="/uploads/cv.pdf">
        <svg aria-hidden="true" viewBox="0 0 24 24"><path d="M14 2H7a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h10a2 2 0 0 0 2-2V7z"></path><path d="M14 2v5h5"></path><path d="M9 13h6"></path><path d="M9 17h6"></path><path d="M9 9h1"></path></svg>
        <span>CV</span>
      </a>
      <a class="profile-link" href="/#contact">
        <svg aria-hidden="true" viewBox="0 0 24 24"><path d="M4 4h16a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2z"></path><path d="m22 6-10 7L2 6"></path></svg>
        <span>Email</span>
      </a>
      <a class="profile-link" href="https://github.com/Bojack-BJ" target="_blank" rel="noopener">
        <svg aria-hidden="true" viewBox="0 0 24 24"><path d="M9 19c-5 1.5-5-2.5-7-3"></path><path d="M15 22v-3.9a3.4 3.4 0 0 0-1-2.6c3.3-.4 6.8-1.6 6.8-7.2a5.6 5.6 0 0 0-1.5-3.9 5.2 5.2 0 0 0-.1-3.9s-1.2-.4-4 1.5a13.8 13.8 0 0 0-7.2 0C5.2-.9 4-.5 4-.5a5.2 5.2 0 0 0-.1 3.9 5.6 5.6 0 0 0-1.5 3.9c0 5.6 3.5 6.8 6.8 7.2a3.4 3.4 0 0 0-1 2.6V22"></path></svg>
        <span>GitHub</span>
      </a>
      <a class="profile-link" href="https://www.linkedin.com/in/xiaotong-li-5635902a3" target="_blank" rel="noopener">
        <svg aria-hidden="true" viewBox="0 0 24 24"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-4 0v7h-4v-7a6 6 0 0 1 6-6z"></path><path d="M2 9h4v12H2z"></path><path d="M4 3a2 2 0 1 1 0 4 2 2 0 0 1 0-4z"></path></svg>
        <span>LinkedIn</span>
      </a>
    </div>
  </aside>

  <div class="home-content">
    <section id="about" class="intro-section">
      <h2>About</h2>
      <p>I am currently working as a VLA model researcher at Lumos Robotics, where I focus on robot manipulation and long-horizon tasks. My recent work includes depth-modality integration for VLA models, mask-guided object-centric manipulation, and improving non-Markovian long-horizon task execution through subtask decomposition and high-level memory modules. More broadly, I am interested in physical world models, VLA models, and robot learning that can understand and interact with the physical world.</p>
      <p>I am seeking PhD opportunities in robotics, especially around physical world models, VLA models, and other related areas.</p>
    </section>

    <section class="education-section">
      <h2>Education</h2>
      <div class="timeline education-list">
        <div>
          <span>2023/09-2025/10</span>
          <p><strong>MSc Robotics, Delft University of Technology</strong></p>
        </div>
        <div>
          <span>2019/09-2023/06</span>
          <p><strong>BEng Aircraft Design and Engineering, Nanjing University of Aeronautics and Astronautics</strong></p>
        </div>
        <div>
          <span>2022/07-2022/08</span>
          <p><strong>Robotics Summer School, Korea Advanced Institute of Science & Technology (KAIST)</strong></p>
        </div>
      </div>
    </section>

    <section id="projects">
      <h2>Selected Projects</h2>
      {% assign projects = site.projects | sort: "date" | reverse %}
      <div class="project-list">
        {% for project in projects %}
          {% assign project_target = project.external_url | default: project.url %}
          <article class="project-item">
            <a class="project-thumb" href="{{ project_target }}" aria-label="{{ project.title }}"{% if project.external_url %} target="_blank" rel="noopener"{% endif %}>
              {% if project.thumbnail %}
                <img src="{{ project.thumbnail }}" alt="">
              {% else %}
                <span>{{ project.date | date: "%Y" }}</span>
              {% endif %}
            </a>
            <div class="project-body">
              <h3><a href="{{ project_target }}"{% if project.external_url %} target="_blank" rel="noopener"{% endif %}>{{ project.title }}</a></h3>
              <p class="project-meta-line">{{ project.date | date: "%Y" }}{% if project.tags %} · {{ project.tags | join: " / " }}{% endif %}</p>
              <p>{{ project.summary }}</p>
              <div class="project-link-row">
                <a href="{{ project_target }}"{% if project.external_url %} target="_blank" rel="noopener"{% endif %}>Project Page</a>
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
      <h2>Working Experience and Internships</h2>
      <div class="timeline experience-list">
        <div>
          <span>2025/12-now</span>
          <p><strong>Embodied AI Researcher</strong>, Lumos Robotics, Suzhou</p>
        </div>
        <div>
          <span>2024/08-2024/12</span>
          <p><strong>Research Intern</strong>, TU Delft Autonomous Multi-Robots Lab, Delft</p>
        </div>
        <div>
          <span>2023/07-2023/08</span>
          <p><strong>ROS Engineer</strong>, Bayer Crop Science, Shanghai</p>
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
