---
---

# Welcome to the AVIS Lab

The **Advanced Vision & Intelligent Systems (AVIS) Lab** at the [Department of Robotics and Mechatronics Engineering](https://www.du.ac.bd/body/RME), [University of Dhaka](https://www.du.ac.bd/), builds AI that can **see, reason, and act** in the physical world.
Led by [Dr. Md Mehedi Hasan]({{ "/team/" | relative_url }}), we work where computer vision, machine learning, and robotics meet.
Our drones navigate with vision-language models. Our agents learn long-horizon behaviour from offline data. Our models diagnose crop and human disease and explain their reasoning.
We publish at venues including Findings of ACL, *PLOS One*, *Plant Methods*, and *IEEE Access*, and partner with agricultural and medical institutions across Bangladesh.

{% include section.html %}

## Latest news

- **Sep 2026:** Two new preprints on offline goal-conditioned RL: [GTRL](https://arxiv.org/abs/2609.33259), and a study asking whether [better goal representations actually help](https://arxiv.org/abs/2609.39901). [Read more]({{ "/2026/09/30/offline-goal-conditioned-rl.html" | relative_url }})
- **May 2026:** [PlantPhenoBot]({{ "/2026/05/07/plantphenobot.html" | relative_url }}), a robotic plant-phenotyping project with Gazipur Agricultural University, begins under a UGC–DU grant.
- **Apr 2026:** [*Thinking Like a Botanist*]({{ "/2026/04/22/thinking-like-a-botanist-acl-2026.html" | relative_url }}) is published in **Findings of ACL 2026**.
- **Apr 2026:** [*VLM-Nav*]({{ "/2026/04/03/vlm-driven-uav-navigation.html" | relative_url }}), mapless UAV navigation driven by vision-language models, is published in **PLOS One**.
- **Jan 2026:** Two papers at **IEEE ICECTE 2026**: [IG-CNN](https://doi.org/10.1109/ICECTE69292.2026.11429443) for knee osteoporosis diagnosis and [FA-EEGNet](https://doi.org/10.1109/ICECTE69292.2026.11429349) for stroke-rehabilitation EEG.
- **Oct 2025:** A MOST-funded project on [explainable AI for histological cancer detection]({{ "/2025/10/19/explainable-ai-histology.html" | relative_url }}) begins with Bangladesh Medical University.

{% include section.html %}

## Highlights

{% capture text %}

We study how machines can perceive and act intelligently, from foundations to deployment. Our areas are **robot learning**, **vision-language reasoning**, **autonomous UAVs**, **plant phenomics**, **medical imaging**, and **intelligent sensing**.
Each area pairs new methods with a concrete problem worth solving: counting wheat spikes in a field, diagnosing a diseased leaf, explaining a cancer prediction to a pathologist.

{%
  include button.html
  link="research"
  text="Explore our research"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/avis-lab.jpeg"
  link="research"
  title="Our Research"
  text=text
%}

{% capture text %}

Our recent work spans Findings of ACL, *PLOS One*, *Plant Methods*, *Smart Agricultural Technology*, *Journal of Building Engineering*, and *IEEE Access*, alongside new preprints in reinforcement learning and vision-language navigation.
Browse every paper since 2022, grouped by year and fully searchable.

{%
  include button.html
  link="publications"
  text="See all publications"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/uav-simulation-town.jpg"
  link="publications"
  title="Publications"
  flip=true
  text=text
%}

{% capture text %}

Our funded projects are supported by MOST, UGC, and ICT, with partners including Gazipur Agricultural University and Bangladesh Medical University.
Running now: **PlantPhenoBot**, a field-robotics project for plant phenotyping, and **explainable AI for cancer pathology**. Past projects range from a teleoperated hospital-assistance robot to plant-disease forecasting.

{%
  include button.html
  link="projects"
  text="Browse our projects"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/field-phenotyping-platform.jpg"
  link="projects"
  title="Our Projects"
  text=text
%}

{% capture text %}

AVIS Lab brings together undergraduate and graduate researchers who work closely with Dr. Hasan from first idea to published paper.
Students lead their own projects, co-author at international venues, and have been recognized with the Faculty of Engineering and Technology **Dean's Award**. Dr. Hasan received one in 2024.

{%
  include button.html
  link="team"
  text="Meet our team"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/dean-awards.jpg"
  link="team"
  title="Our Team"
  flip=true
  text=text
%}
