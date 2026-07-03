---
title: Building Explicit World Model for Open-world Object Manipulation
date: 2025-10-01
summary: A manipulation framework that combines open-set perception, 3D digital twin reconstruction, and simulation-based strategy sampling without task-specific action demonstrations.
tags:
  - Open-world manipulation
  - World model
  - Robotics
thumbnail: /images/thesis.png
links:
  - label: Thesis PDF
    url: /uploads/Thesis.pdf
---

<video class="project-main-video" controls playsinline poster="/images/thesis.png" src="/uploads/thesis.mp4"></video>

<div class="video-strip">
  <video autoplay muted loop playsinline src="/uploads/lemon-cup.MOV"></video>
  <video autoplay muted loop playsinline src="/uploads/cube-box.MOV"></video>
  <video autoplay muted loop playsinline src="/uploads/cube-can.MOV"></video>
  <video autoplay muted loop playsinline src="/uploads/banana-basket.mp4"></video>
  <video autoplay muted loop playsinline src="/uploads/cup-box.mp4"></video>
</div>

Open-world object manipulation has emerged as a popular research frontier in robotics. While recent vision-language-action models have achieved impressive results, they typically rely on large amounts of task-specific action data for training. This project explores a different route: enabling a manipulator to perform open-world manipulation tasks by understanding object dynamics rather than imitating action demonstrations.

![System overview](/images/thesis.png)

The framework integrates open-set segmentation and grasping, 3D digital twin reconstruction, and simulation-based strategy sampling. A physically grounded digital twin allows the robot to simulate and evaluate possible interaction strategies before real-world execution.

The system was tested on tasks such as putting a banana into a basket, stacking cubes, and placing a cup upside down on a box. These tasks were completed without task-specific action demonstrations, highlighting the potential of explicit world models for generalization.

## Demonstrations

<div class="media-grid">
  <figure>
    <video controls src="/uploads/lemon-cup.MOV"></video>
    <figcaption>Put lemon into cup</figcaption>
  </figure>
  <figure>
    <video controls src="/uploads/cube-box.MOV"></video>
    <figcaption>Put cube into box</figcaption>
  </figure>
  <figure>
    <video controls src="/uploads/stack_cube.mp4"></video>
    <figcaption>Stack two cubes</figcaption>
  </figure>
  <figure>
    <video controls src="/uploads/cup1.MOV"></video>
    <figcaption>Put cup upside down on box</figcaption>
  </figure>
</div>
