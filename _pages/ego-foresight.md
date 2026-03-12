---
layout: distill
permalink: /ego-foresight/
nav: false
title: Ego-Foresight
description: Self-supervised Learning of Agent-Aware Representations for Improved RL
tags: distill formatting
giscus_comments: false
date: 2026-02-18
featured: true
mermaid:
  enabled: true
  zoomable: true
code_diff: true
map: true
chart:
  chartjs: true
  echarts: true
  vega_lite: true
tikzjax: true
typograms: true

authors:
  - name: Manuel Serra Nunes
    affiliations:
      name: Técnico Lisboa
  - name: Atabak Dehban
    affiliations:
      name: Técnico Lisboa
  - name: Yiannis Demiris
    affiliations:
      name: Imperial College London
  - name: José Santos-Victor
    affiliations:
      name: Técnico Lisboa

bibliography: 2018-12-22-distill.bib
---

## Abstract

Despite the significant advances in Deep Reinforcement Learning (RL) observed
in the last decade, the amount of training experience necessary to learn effective
policies remains one of the primary concerns in both simulated and real environments. Looking to solve this issue, previous work has shown that improved
efficiency can be achieved by separately modeling the agent and environment, but
usually requires a supervisory signal. In contrast to RL, humans can perfect a new
skill from a small number of trials and often do so without a supervisory signal,
making neuroscientific studies of human development a valuable source of inspiration for RL. In particular, we explore the idea of motor prediction, which states
that humans develop an internal model of themselves and of the consequences that
their motor commands have on the immediate sensory inputs. Our insight is that
the movement of the agent provides a cue that allows the duality between the agent
and environment to be learned. To instantiate this idea, we present Ego-Foresight
(EF), a self-supervised method for disentangling agent information based on motion and prediction. Our main finding is that, when used as an auxiliary task in
feature learning, self-supervised agent-awareness improves the sample-efficiency
and performance of the underlying RL algorithm. To test our approach, we study
the ability of EF to predict agent movement and disentangle agent information.
Then, we integrate EF with model-free and model-based RL algorithms to solve
simulated control tasks, showing improved sample-efficiency and performance.
