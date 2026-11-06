---
title: "Reaching goals from offline data: GTRL and the goal-representation question"
image: images/gtrl-method.jpg
tags:
  - ongoing
  - reinforcement learning
  - robot learning
---

Can an agent learn to reach *any* goal, across long horizons, using nothing but a fixed dataset of past experience?
That is the question behind our newest line of work in **offline goal-conditioned reinforcement learning (GCRL)**. In September 2026 we released two preprints on it.

**At a glance**

- **Status:** Ongoing research
- **Area:** Robot learning, reinforcement learning
- **Papers:** [GTRL (arXiv 2026)](https://arxiv.org/abs/2609.33259) · [Do Better Goal Representations Improve GCRL? (arXiv 2026)](https://arxiv.org/abs/2609.39901)

{% include section.html %}

## GTRL: grounding divide-and-conquer with temporal differences

Divide-and-conquer value learning scales to long horizons by joining two shorter segments at a subgoal.
It has two blind spots, though. Under stochastic dynamics, its base case ends up valuing the *luckiest* trajectories in the data. And a state–goal pair that no logged trajectory connects never receives a value update at all.

**GTRL (Grounded Transitive RL)** fixes both by adding a one-step temporal-difference (TD) target to the composition.
Over a single step TD is correct: its target averages over successor states and needs no subgoal.
With that addition every pair receives an update, and the composition still carries the long horizon.
GTRL also corrects the bias introduced by hindsight relabeling by reweighting each goal according to how reachable it was from other successors.
Across nineteen OGBench tasks spanning stochastic, deterministic, and stitching environments, GTRL achieves the highest average success rate.

{%
  include figure.html
  image="images/gtrl-method.jpg"
  caption="GTRL's two components on a maze. **(a) Counterfactual goals:** the plain transitive update (TRL) reaches only 33% of states for goal *g*; GTRL updates every state. **(b) Hindsight weighting:** relabeled goals reflect only the outcome that happened, and GTRL's weight restores the spread of outcomes that were reachable."
  width="100%"
%}

*Abdul Monaf Chowdhury, MD Sameer Iqbal Chowdhury, Shifat E Arman, Md Mehedi Hasan.* [arXiv:2609.33259](https://arxiv.org/abs/2609.33259)

## Is the goal representation really the bottleneck?

Much recent GCRL research focuses on better ways to encode goals, using temporal distance, occupancy, or controllability. We asked how much that actually matters.

We built an *exact* temporal-distance goal representation in deterministic mazes, then systematically corrupted it while keeping the downstream learner fixed.
Large changes in goal-representation quality produced almost no change in performance.
The same interventions applied to the agent's **current state**, however, more than doubled success. The state pathway is the real bottleneck.
Building on that finding, simple random Fourier positional encodings of the state substantially improve performance on the hardest navigation tasks, with no map information and no change to the objective.

*Syed Nazmus Sakib, Abdul Monaf Chowdhury, Nafiul Haque, Shifat E Arman, Md Mehedi Hasan.* [arXiv:2609.39901](https://arxiv.org/abs/2609.39901)

## What's next

Code for both papers will be released soon.
In parallel, lab members are working on long-horizon, multi-task embodied manipulation, which is where better offline value learning pays off most.
