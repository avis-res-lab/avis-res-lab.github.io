---
title: "PlantPhenoBot: robotics for plant phenotyping"
image: images/field-phenotyping-platform.jpg
tags:
  - ongoing
  - robotics
  - plant phenomics
---

**PlantPhenoBot** is the lab's newest funded project. It is a robotics project for plant phenotyping, the measurement of plant traits such as growth, architecture, and stress response.
The project began in May 2026 under a UGC–DU research grant, in collaboration with **Gazipur Agricultural University**.

**At a glance**

- **Status:** Ongoing (started 7 May 2026)
- **Funding:** UGC–DU research grant
- **Collaborator:** Gazipur Agricultural University
- **Principal investigator:** Dr. Md Mehedi Hasan
- **Area:** Robotics, plant phenomics

{% include section.html %}

## Why phenotyping needs robots

Crop breeders choose new varieties by measuring traits plant by plant: how fast a plant grows, how many spikes or bolls it sets, and how it copes with drought, heat, or disease.
Done by hand, this is slow, subjective, and hard to scale beyond a few plots.
Robots and imaging platforms can collect the same measurements automatically and consistently, at far higher throughput. This is *high-throughput phenotyping*, and it is one of the main bottlenecks between plant science and better crops.

{%
  include figure.html
  image="images/field-phenotyping-platform.jpg"
  caption="A land-based imaging platform for field wheat phenotyping, as shown in the lab's WheatSpikeNet study (Batin et al., *Frontiers in Plant Science*, 2023; CC BY 4.0)."
  width="100%"
%}

## Building on years of phenotyping work

PlantPhenoBot draws on a long line of AVIS Lab research in plant phenomics:

- **Wheat spike detection and segmentation.** Dr. Hasan's 2018 *Plant Methods* paper on detecting wheat spikes with CNNs, followed by [WheatSpikeNet](https://doi.org/10.3389/fpls.2023.1226190) (*Frontiers in Plant Science*, 2023) and a multi-stage CNN for spike analysis (*DUJASE*, 2023).
- **Seedling monitoring.** [Cotton seedling growth-stage classification](https://doi.org/10.1016/j.atech.2025.101619) from UAV and ground-level imagery, with a biologically grounded Composite Stress Index (*Smart Agricultural Technology*, 2025).
- **Disease diagnosis.** [PlantCareNet](https://doi.org/10.1186/s13007-025-01366-9) (*Plant Methods*, 2025) and [SugarcaneShuffleNet](https://arxiv.org/abs/2508.17107), a very fast model for on-device diagnosis of sugarcane leaf diseases.
- **Expert-style reasoning.** [PlantInquiryVQA](https://doi.org/10.18653/v1/2026.findings-acl.1741) (*Findings of ACL 2026*), a benchmark that tests whether multimodal models can question a leaf image the way a botanist does.

We'll post updates here as the project progresses.
