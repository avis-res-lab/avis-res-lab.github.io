---
title: "Flying with one camera: vision-language models for UAV navigation"
image: images/uav-simulation-town.jpg
tags:
  - ongoing
  - uav
  - vision-language models
---

Most autonomous drones avoid obstacles with expensive sensors, a prebuilt map, or both.
Our UAV research asks how far a drone can get with a **single monocular camera** and a **vision-language model (VLM)** that reasons about what it sees.
The first answer, **VLM-Nav**, was published in *PLOS One* in April 2026. A sim-to-real follow-up is now available as a preprint.

**At a glance**

- **Status:** Ongoing research
- **Area:** Autonomous UAVs, vision-language models
- **Papers:** [VLM-Nav (PLOS One, 2026)](https://doi.org/10.1371/journal.pone.0345778) · [Cross-modal benchmarking with sim-to-real evaluation (SSRN preprint, 2026)](https://doi.org/10.2139/ssrn.7374301)

{% include section.html %}

## VLM-Nav: mapless navigation from monocular vision

VLM-Nav converts each RGB frame from the drone into a depth map using **DepthAnything-V2**, a zero-shot depth estimator.
A VLM (the study explores Gemini-flash and GPT-4o) reads the depth map, detects nearby obstacles, and proposes an avoidance manoeuvre.
A small fully connected network then combines the VLM's output with the UAV's heading relative to its target and picks the next action.
No map is needed, and the hardware is cheap.

{%
  include figure.html
  image="images/vlm-nav-drone.jpg"
  caption="The UAV setup in VLM-Nav: a forward-facing monocular camera (90° field of view) plus GPS, altitude, and side distance sensors. Sarker et al., *PLOS One*, 2026 (CC BY 4.0)."
  width="100%"
%}

*Gobinda Chandra Sarker, AKM Azad, Sejuti Rahman, Md Mehedi Hasan.* This builds on Gobinda's MSc thesis on monocular, depth-based UAV navigation in 3D terrain (2024).

## From simulation to a real quadrotor

The follow-up study moves the reasoning off the aircraft. The UAV streams live video to a ground station, which fuses monocular depth with a VLM and sends back discrete **MAVLink** commands.

- **In simulation:** six contemporary VLMs were benchmarked across nine factorially controlled **Unity–ROS 2** scenes, covering 265 episodes and 3,383 logged decisions.
- **In flight:** three cloud VLMs and a non-learning heuristic baseline were flown on a **Pixhawk 6C** quadrotor, with 1,568 decisions recorded for each.

Every reported proportion comes with a Wilson 95% confidence interval and a significance test.
The work grew out of the 2025 student project *Advancing UAV Flight and Obstacle Avoidance with Cross-Modal Deep Learning Integration*.

*Abyead Zarif Hassan, Samiha Tarannum Noor, AKM Azad, Md Mehedi Hasan.*

## Earlier UAV work

Earlier UAV work in the lab focused on aerial perception. Projects included object and intrusion detection from UAVs, and human-action recognition from drone video with [FFT-UAVNet](https://doi.org/10.1109/sti59863.2023.10465205) (2023) and [U-ActionNet](https://doi.org/10.1109/ACCESS.2024.3516586) (*IEEE Access*, 2024).
