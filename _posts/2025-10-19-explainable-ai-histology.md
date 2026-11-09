---
title: "Explainable AI for histological cancer detection"
image: images/histology-cancer-detection.png
tags:
  - ongoing
  - medical ai
  - explainable ai
---


Deep learning can now classify microscopic tissue images with high accuracy, but pathologists rarely trust a model that cannot show *why* it reached a decision.
This project builds cancer-detection models that are both accurate and interpretable. It is funded by the **Ministry of Science and Technology (MOST)** and runs in collaboration with **Bangladesh Medical University (BMU)**.

**At a glance**

- **Project:** Enhancing Histology Cancer Cell Detection: Deep Learning Model Interpreted with eXplainable AI (XAI) for Microscopic Tissue Image Analysis
- **Status:** Ongoing (started 19 October 2025)
- **Funding:** Ministry of Science and Technology (MOST), Bangladesh
- **Collaborator:** Bangladesh Medical University (BMU)
- **Principal investigator:** Dr. Md Mehedi Hasan

{% include section.html %}

## The approach

The project builds on a 2024 student research project of the same name by Shamaeta Paul Gupta and Apurba Roy.
The resulting framework [(preprint)](https://doi.org/10.21203/rs.3.rs-8157817/v1):

- combines an **ensemble of three pretrained CNNs**: ResNet50, VGG16, and InceptionV3;
- uses a **4× super-resolution** step to sharpen tissue images before classification, which improved accuracy by 1–10% (ResNet50 96.21%, VGG16 92.14%, InceptionV3 96.42%);
- explains each prediction with **Grad-CAM, SHAP, and LIME**, so clinicians can see which regions and features drove the decision.

The MOST-funded project continues this work with clinical collaborators at BMU.

## Related medical-AI work in the lab

- **Explainable vision-language models for medical reports.** An ongoing MPhil project (Md Julhas Hossain) is building a framework that automatically interprets diagnostic medical reports and explains them to patients.
- **Bone health from X-rays.** [IG-CNN](https://doi.org/10.1109/ICECTE69292.2026.11429443) (IEEE ICECTE 2026) and a follow-up preprint apply information-geometric deep learning to knee osteoporosis diagnosis.
- **Biosignals.** [FA-EEGNet](https://doi.org/10.1109/ICECTE69292.2026.11429349) classifies stroke-rehabilitation movements from EEG, and a 2025 student project explored an EEG-actuated bionic hand.
