---
title: Model Predictive Control Approach for Multi-UAVs Planning and Motion Control
date: 2024-04-01
summary: A model predictive control approach for trajectory tracking, collision avoidance, and planning of multiple UAVs in complex environments.
tags:
  - MPC
  - UAV
  - Planning
thumbnail: /images/terminalset_visual.png
links:
  - label: GitHub
    url: https://github.com/PatrickYang-5/MPC_drones
  - label: Report PDF
    url: /uploads/mpc.pdf
---

![MPC experiment result](/images/punish.png)
![Terminal set visualization](/images/terminalset_visual.png)

We implemented and simulated a model predictive control approach for multi-UAV control. A state-based MPC controller for single-UAV position control was first designed and used to study parameter effects. We then developed a path-planning method and output MPC strategy for trajectory tracking and collision avoidance with multiple UAVs in complex environments.

A stability analysis was also performed to reason about controller behavior.
