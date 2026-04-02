---
layout: single
title: "" # Leave empty
author_profile: true
permalink: /projects/predictability/
toc: true
toc_sticky: true
toc_label: "Page Contents"
excerpt: >
  <div style="text-align: center; max-width: 90%; margin: 0 auto;">
    <span style="display: block; font-size: 2.0em; font-weight: bold; color: white; line-height: 1.2;">
      <span style="opacity: 0.7; font-size: 0.8em;">Projects &rsaquo;</span> Predictability
    </span>
  </div>
header:
  overlay_color: "#000"
  overlay_filter: 0.1
  overlay_image: https://raw.githubusercontent.com/mmistakes/minimal-mistakes/master/assets/images/header-bg.jpg
---

<div class="notice--info">
  <strong>Status: Ongoing Project</strong><br>
  The first phase of this project focused on the logistic map's predictability properties and is completed. Please refer to the specific details below.
</div>

## Overview
While Data Assimilation focuses on optimizing the *current* state of the atmosphere, **Predictability** research asks a more fundamental question: *Regardless of how good our initial data is, what is the theoretical limit of our ability to forecast the future?*

My research in this area explores the boundaries of chaotic systems, focusing on error growth, the "butterfly effect," and the intrinsic limits of prediction in non-linear dynamical systems.

## Key Research Themes

### 1. The Limit of Predictability
My recent work challenges standard definitions of predictability by utilizing the **Logistic Map**—a classic example of a simple system exhibiting complex chaotic behavior—to mathematically define the "limit of predictability."

This research investigates how error growth rates (Lyapunov exponents) interact with initial condition uncertainty to determine the time horizon beyond which a forecast provides no more value than a climatological guess.

* **Aksoy, A. (2024).** The logistic map: A possible definition of the limit of predictability? *Chaos*, 34, 013106. [doi:10.1063/5.0181705](https://doi.org/10.1063/5.0181705)

### 2. Ensemble Spread & Error Growth
In the context of tropical cyclones, understanding predictability requires analyzing how initial errors grow over time. Through my work with **Ensemble Kalman Filters (EnKF)**, I examine how ensemble spread correlates with forecast error, serving as a proxy for the flow-dependent predictability of the atmosphere.

* **Aksoy, A. et al. (2022).** Tropical cyclone data assimilation with Coyote uncrewed aircraft system observations, very frequent cycling, and a new online quality control technique. *Mon. Wea. Rev.* [doi:10.1175/MWR-D-21-0124.1](https://doi.org/10.1175/MWR-D-21-0124.1)

## Interactive Tools
To demonstrate these theoretical concepts, I developed the **Logistic Map Explorer**, an interactive web application that allows users to visualize the "butterfly effect" and error growth in real-time.

<div style="margin-top: 20px; margin-bottom: 30px; padding: 20px; background-color: #f2f2f2; border-radius: 5px;">
  <h3 style="margin-top: 0; text-align: center;">Try the Simulation</h3>
  <ul>
    <li style="margin-bottom: 15px;">
      Run the model in your browser to explore bifurcation diagrams: 
      <br><br>
      <a href="https://logistic-map-v1.streamlit.app/" class="btn btn--primary btn--sm" style="margin-left: 10px; vertical-align: middle;">Launch Streamlit App <i class="fas fa-external-link-alt"></i></a>
      <a href="https://github.com/aaksoy-umiami/logistic_map" class="btn btn--inverse btn--sm" style="margin-left: 10px; vertical-align: middle;"><i class="fab fa-github"></i> View Source Code</a>
    </li>
    <li>
      <em>Want to understand the math?</em> Visit the <a href="/tools/logistic-map/">Tool Documentation & Tutorial</a> page for a detailed breakdown of the physics and source code.
    </li>
  </ul>
</div>

---
**[← Back to Projects](/projects/)** |  [Go to Home](/)
