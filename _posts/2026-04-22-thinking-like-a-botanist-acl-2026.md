---
title: "Thinking Like a Botanist: PlantInquiryVQA in Findings of ACL 2026"
image: images/thinking-botanist.jpg
tags:
  - publication
  - vision-language models
  - plant phenomics
---

Our paper *Thinking Like a Botanist: Challenging Multimodal Language Models with Intent-Driven Chain-of-Inquiry* is published in **Findings of the Association for Computational Linguistics: ACL 2026**.
It introduces **PlantInquiryVQA**, a benchmark that asks whether multimodal AI can reason about a plant the way an expert does, one targeted question at a time.

**At a glance**

- **Venue:** Findings of ACL 2026
- **Dataset:** 24,950 expert-curated plant images · 138,068 question–answer pairs
- **Links:** [ACL Anthology](https://doi.org/10.18653/v1/2026.findings-acl.1741) · [arXiv](https://arxiv.org/abs/2604.20983)

{% include section.html %}

## The problem: one question is not a diagnosis

A botanist examining a diseased leaf does not answer a single question and stop.
They spot visual cues, form a hypothesis about what is going on, and ask follow-up questions that adapt to the species, the symptoms, and the severity.
That structured probing is what makes their diagnoses accurate and their treatment advice safe.
Vision-language models, however, are almost always evaluated on single-turn question answering.

## What we built

- **Chain of Inquiry.** A framework that models a diagnosis as an ordered sequence of questions and answers, each conditioned on grounded visual cues and an explicit diagnostic intent.
- **PlantInquiryVQA.** 24,950 expert-curated plant images and 138,068 question–answer pairs, annotated with visual grounding, severity labels, and domain-specific reasoning templates.

{%
  include figure.html
  image="images/thinking-botanist.jpg"
  caption="How PlantInquiryVQA is built: visual cue extraction, Chain-of-Inquiry classification, and automated question–answer generation with expert review."
  width="100%"
%}

## What we found

Top-tier multimodal large language models describe visual symptoms reasonably well, but they **struggle with safe clinical reasoning and accurate diagnosis**.
Guiding them through structured, question-led inquiry significantly improves diagnostic correctness, reduces hallucination, and makes their reasoning more efficient.
We hope PlantInquiryVQA helps the community train diagnostic agents that reason like expert botanists rather than act as static classifiers.

*Syed Nazmus Sakib, Nafiul Haque, Shahrear Bin Amin, Hasan Muhammad Abdullah, Md. Mehedi Hasan, Mohammad Zabed Hossain, Shifat E. Arman.*
