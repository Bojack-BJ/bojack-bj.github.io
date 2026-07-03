---
title: Gradient Enhanced Neural Networks for Optimization of Mars Low Reynold Number Airfoil
date: 2023-04-01
summary: A surrogate-modeling approach that uses gradient-enhanced neural networks to accelerate low-Reynolds-number airfoil optimization.
tags:
  - Optimization
  - Surrogate model
  - Aerodynamics
thumbnail: /images/gradient3.jpg
links:
  - label: Chinese Thesis PDF
    url: /uploads/paper.pdf
---

This project uses an improved gradient-enhanced neural network as a surrogate model instead of CFD simulation to predict aerodynamic parameters of airfoils. We compared traditional neural networks, gradient-enhanced neural networks, and improved gradient-enhanced neural networks to evaluate prediction performance and convergence speed.

<figure>
  <img src="/images/gradient1.jpg" alt="Accuracy and convergence comparison">
  <figcaption>Accuracy and convergence of different networks.</figcaption>
</figure>

For preprocessing, singular value decomposition was used to parameterize airfoils into modes and modal coefficients. Inverse-distance-weighted interpolation was used to construct a constraint function for modal coefficients and exclude abnormal airfoils.

<figure>
  <img src="/images/gradient2.jpg" alt="SVD airfoil modes">
  <figcaption>The first five airfoil camber and thickness modes from SVD decomposition of the UIUC airfoil database.</figcaption>
</figure>

Latin hypercube sampling was used to generate airfoil samples, and ADflow was used to calculate aerodynamic parameters and derivatives. The trained surrogate model was coupled with an optimization package for airfoil aerodynamic optimization. Compared with high-fidelity CFD-based optimization, the result was similar while the optimization time was greatly reduced.

<figure>
  <img src="/images/gradient3.jpg" alt="Airfoil grids computed by pyHyp">
  <figcaption>Airfoil grids computed by pyHyp.</figcaption>
</figure>
