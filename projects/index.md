---
title: Projects
nav:
  order: 3
  tooltip: Funded projects and research lines
---

# {% include icon.html icon="fa-solid fa-wrench" %}Projects

The lab's funded projects and active research lines, supported by the Ministry of Science and Technology (MOST), the University Grants Commission (UGC), and ICT, with partners including Gazipur Agricultural University and Bangladesh Medical University.
Click any project for the full story on our [Blog]({{ "/blog/" | relative_url }}).

{% include tags.html tags="ongoing, completed, robotics, uav, plant phenomics, medical ai, reinforcement learning" %}

{% include search-info.html %}

{% include section.html %}

## Running now

{% include list.html component="card" data="projects" filter="group == 'featured'" %}

{% include section.html %}

## Completed

{% include list.html component="card" data="projects" filter="!group" style="small" %}

{% include section.html %}

## Code & data

Code and datasets are linked from the individual papers on our [Publications]({{ "/publications/" | relative_url }}) page where available.
