---
title: "9-DoF Tendon-Driven Dexterous Hand with Force-Feedback Exoskeleton"
excerpt: >
  High-backdrivability dexterous hand and matched force-feedback exoskeleton for teleoperation and contact-rich manipulation.
header:
  teaser: /images/dexterous-hand-teaser.png   # add your teaser image to /images/
collection: portfolio
# show_in_portfolio: false  # set to false to hide from portfolio page
---

## Overview

Designed a **9-DoF tendon-driven dexterous hand** actuated by BLDC motors with FOC control for high backdrivability and torque transparency. Built a matched **9-DoF force-feedback exoskeleton** for teleoperation and multimodal data collection. Implemented current-based torque estimation and tendon transmission modeling for real-time force sensing. Developing a synchronized pipeline capturing joint states, motor currents, and estimated contact forces for contact-rich manipulation and force-aware imitation learning.

*This project is currently in progress.*

---

## Media

*Add your images and videos below using the `portfolio-media` include. Put files in `/images/` (or `/files/` for larger videos), then fill in the paths and captions.*

### Image example

{% include portfolio-media.html path="/images/dexterous-hand-1.png" caption="9-DoF tendon-driven hand prototype with BLDC motors and FOC drivers." width="800" %}

### Video example

{% include portfolio-media.html path="/images/dexterous-hand-demo.mp4" type="video" caption="Teleoperation demo: hand and exoskeleton force feedback." width="800" %}

*To add more: copy one of the blocks above, change `path` to your file (e.g. `path="/images/your-photo.png"` or `path="/files/your-video.mp4"`), set `caption="Your caption"`, and optionally `width="800"`. For video use `type="video"`.*

---

## Technical highlights

- **Hand:** 9-DoF, tendon-driven, BLDC motors with FOC for backdrivability and torque transparency  
- **Exoskeleton:** 9-DoF force feedback for teleoperation and data collection  
- **Sensing:** Current-based torque estimation, tendon transmission modeling, real-time force sensing  
- **Pipeline (in development):** Synchronized joint states, motor currents, estimated contact forces for contact-rich manipulation and force-aware imitation learning
