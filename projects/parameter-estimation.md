---
layout: single
title: "" # Leave empty
author_profile: true
permalink: /projects/parameter-estimation/
toc: true
toc_sticky: true
toc_label: "Page Contents"
excerpt: >
  <div style="text-align: center; max-width: 90%; margin: 0 auto;">
    <span style="display: block; font-size: 2.0em; font-weight: bold; color: white; line-height: 1.2;">
      <span style="opacity: 0.7; font-size: 0.8em;">Projects &rsaquo;</span> Parameter Estimation
    </span>
  </div>
header:
  overlay_color: "#000"
  overlay_filter: 0.1
  overlay_image: https://raw.githubusercontent.com/mmistakes/minimal-mistakes/master/assets/images/header-bg.jpg
---

<div class="notice--info">
  <strong>Status: Completed Project</strong><br>
  This work was my Ph.D. research and is now completed. Please refer to the specific details below.
</div>

## Overview
A significant portion of my research, originating from my Ph.D. work, focuses on **Parameter Estimation**—the use of data assimilation techniques not just to correct the atmospheric state (wind, temperature), but to objectively optimize the underlying model parameters (friction, mixing coefficients) that govern physical processes.

This work demonstrated that the **Ensemble Kalman Filter (EnKF)** could successfully estimate uncertain parameters in complex mesoscale models, effectively reducing model error and improving forecast skill.

## Key Research Themes

### 1. Simultaneous State & Parameter Estimation
My early work pioneered the use of EnKF for simultaneous state and parameter estimation in mesoscale models. We demonstrated that uncertain physical parameters (such as surface drag or vertical mixing coefficients) could be retrieved from standard observations, leading to more balanced and accurate analyses.

* **Aksoy, A., F. Zhang, and J. W. Nielsen-Gammon (2006).** Ensemble-based simultaneous state and parameter estimation with MM5. *Geophys. Res. Lett.* [doi:10.1029/2006GL026186](https://doi.org/10.1029/2006GL026186)
* **Aksoy, A., F. Zhang, and J. W. Nielsen-Gammon (2006).** Ensemble-based simultaneous state and parameter estimation in a two-dimensional sea-breeze model. *Mon. Wea. Rev.* [doi:10.1175/MWR3224.1](https://doi.org/10.1175/MWR3224.1)
* **Aksoy et al. (2005).** Ensemble-based data assimilation for thermally forced circulations. *J. Geophys. Res. Atmos.* [doi:10.1029/2004JD005718](https://doi.org/10.1029/2004JD005718)

### 2. Encyclopedia Entries
I was invited to author the definitive entry on "Parameter Estimation" for the *Encyclopedia of Atmospheric Sciences*. I have maintained this entry across multiple editions, synthesizing the state-of-the-art in parameter estimation theory and its practical application in mitigating model error.

* **Aksoy, A. (2025).** Parameter Estimation. In *Encyclopedia of Atmospheric Sciences* (3rd ed.). (Eds. W. A. Robinson & P. Yang). Academic Press. [Link to Publisher](https://www.sciencedirect.com/referencework/9780123822253/encyclopedia-of-atmospheric-sciences)
* **Aksoy, A. (2015).** Parameter Estimation. In *Encyclopedia of Atmospheric Sciences* (2nd ed., Vol. 4, pp. 181–186). (Eds. G. R. North, J. Pyle, & F. Zhang). Academic Press.

## Related Applications
* [Predictability](/projects/predictability/): Exploring how parameter uncertainty impacts the intrinsic predictability of chaotic systems.

---
**[← Back to Projects](/projects/)** |  [Go to Home](/)
