---
title: Research
nav:
  order: 1
  tooltip: Research areas and highlighted work
---

# {% include icon.html icon="fa-solid fa-microscope" %}Research

The **AVIS Lab** builds intelligent systems that perceive the world through cameras and sensors, reason about what they see, and act on it.
Our work runs from foundations to deployment. On the foundations side we develop new learning algorithms, optimizers, and visual tokenizers. On the deployment side our systems fly drones, diagnose crop and human disease, and control assistive devices.
We care equally about the science and the real-world result. Much of our work starts with a problem in Bangladesh, such as a field disease, a hospital workflow, or a sensing gap, and ends as a model, a dataset, or a working prototype.

{% include section.html %}

## Research areas

### {% include icon.html icon="fa-solid fa-robot" %}Robot learning & embodied intelligence

How should a robot decide how, when, and where to move? We study **offline goal-conditioned reinforcement learning**, where agents learn long-horizon, goal-reaching behaviour purely from logged data.
Recent work includes *GTRL*, which grounds divide-and-conquer value learning with temporal differences, and a study showing that the agent's state representation, not the goal representation, is the real bottleneck.
This line builds on Dr. Hasan's industrial experience with **vision-based robot control** (visual servoing, tool pick-up, and placement). It extends to compliant grasping and sensor-driven prosthetic hands.

### {% include icon.html icon="fa-solid fa-comments" %}Vision-language models & multimodal reasoning

Large vision-language models describe images well but often reason poorly about them. We build benchmarks and methods that test and improve **multi-step, grounded visual reasoning**.
*PlantInquiryVQA* (Findings of ACL 2026) evaluates whether models can question a leaf image the way an expert botanist does.
Related work covers counting objects hidden behind occluders, non-neural visual tokenization, and explainable vision-language systems for medical reports.

### {% include icon.html icon="fa-solid fa-helicopter" %}Autonomous UAVs

We want drones that can fly safely with nothing more than a single camera. **VLM-Nav** (PLOS One, 2026) turns monocular images into depth maps and lets a vision-language model plan collision-free manoeuvres without a prebuilt map.
A follow-up benchmarks six VLMs in Unity–ROS 2 simulation and flight-tests them on a Pixhawk 6C quadrotor.
Earlier work recognizes human actions from aerial video for drone surveillance (*U-ActionNet*, *FFT-UAVNet*).

### {% include icon.html icon="fa-solid fa-seedling" %}Plant phenomics & precision agriculture

Plant phenotyping measures traits such as growth, architecture, yield, and stress tolerance, the quantitative basis of crop breeding.
We use field imaging, UAVs, and deep learning to measure these traits automatically. Examples include detecting and segmenting wheat spikes (*WheatSpikeNet*), classifying cotton seedling growth stages from UAV imagery, and diagnosing plant diseases with lightweight on-device models (*PlantCareNet*, *SugarcaneShuffleNet*).
Our current project, **PlantPhenoBot**, brings robotics into the field with Gazipur Agricultural University.

### {% include icon.html icon="fa-solid fa-heart-pulse" %}Medical imaging & biomedical AI

Clinicians need AI they can trust. We develop interpretable models for medical images and biosignals.
This includes information-geometric networks for knee osteoporosis from X-rays and **explainable AI for histological cancer detection** (a MOST-funded project with Bangladesh Medical University). On the biosignal side we work on EEG decoding for stroke rehabilitation and on brain–computer interfaces for prosthetic control.

### {% include icon.html icon="fa-solid fa-microchip" %}Intelligent sensing, IoT & learning foundations

We pair smart sensors with machine learning for environmental and industrial condition monitoring. Examples include IoT-driven energy forecasting for commercial buildings, landslide-risk prediction from climate projections, and real-time face recognition for video surveillance.
Alongside these applications we work on the learning machinery itself: new optimizers (*SPARK*), loss functions (*AGL Loss*), and physics-informed machine learning for classifying celestial objects.

{% include section.html %}

## Highlighted publications

Selected recent work: new algorithms, a Findings of ACL paper, and articles in leading journals.

{% include citation.html lookup="arxiv:2609.33259" style="rich" %}

{% include citation.html lookup="doi:10.18653/v1/2026.findings-acl.1741" style="rich" %}

{% include citation.html lookup="doi:10.1371/journal.pone.0345778" style="rich" %}

{% include citation.html lookup="doi:10.1186/s13007-025-01366-9" style="rich" %}

{% include citation.html lookup="doi:10.1016/j.atech.2025.101619" style="rich" %}

{% include citation.html lookup="doi:10.1016/j.jobe.2025.113315" style="rich" %}

{% include section.html %}

## All publications

Every paper from 2022 onward, grouped by year and searchable, is on the Publications page.

{%
  include button.html
  link="publications"
  text="Browse all publications"
  icon="fa-solid fa-arrow-right"
  flip=true
%}
{%
  include button.html
  type="google-scholar"
  text="Google Scholar"
  link="https://scholar.google.com/citations?hl=en&user=jGC1OfgAAAAJ&view_op=list_works&sortby=pubdate"
%}
