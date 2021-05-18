---
title: Introduction to Causal Inference for Program Evaluation
author: Wesley Furlong
date: '2021-05-18'
slug: introduction-to-causal-inference-for-program-evaluation
categories: []
tags: []
subtitle: ''
summary: ''
authors: []
lastmod: '2021-05-18T11:55:50-04:00'
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---

**What is a causal effect?**

The goal of this post is to distinguish a causal effect in program evaluation from a simple difference calculated from a pre-post test and introduce a few of the primary causal estimates that might be of interest in program evaluation.

Causal effects describe the expected change in outcome due to an intervention (e.g., program, treatment) *when compared with a baseline condition.* For example, take a clinical program for foster youth where trauma-informed cognitive behavioral therapy and EMDR (eye movement desensitization and reprocessing) are both used with clients. Which shows better results? Should both be used? Or, what if it depends on factors like age or level of trauma? Ideally, we might want to know if certain subgroups receive different benefits from a treatment compared with others.

To answer these causal questions, we need to know the difference for the child *with and without the treatment.* Unfortunately, this cannot be accomplished with a simple difference of scores before and after a treatment.

**Why not just pre-post test?**

By itself, a pre-post test cannot yield a causal estimate because it does not answer the question, "What would have occurred without the treatment?" The person may have improved without the treatment. Many factors may influence the pre-post scores. We need to distinguish two potential outcomes for the same person: when treated - when untreated.

> Impact = factual (what happened) - counterfactual (what would happen minus the treatment/intervention)

![](simple_difference.png)

Of course, it's impossible to identify more than one outcome for a single person. However, for programs, we can estimate causal effects under certain conditions.

![](counterfactual.png)

The gold standard is a randomized controlled trial where, providing the assumptions are met, the average treatment effect is simply the difference between the treated and controlled group.

When we work with observational data where individuals are not randomly selected and placed into treatment and control, we aim to model experimental conditions, including randomization. One way to address potential selection bias from a non-randomized sample is by carefully creating the control and treated groups with propensity scores. In future posts, we will dive deeper into propensity scores and the various methods for calculating them. For now, I want to distinguish three relevant types of causal effect estimates for program evaluation:

1.  Average treatment effect (ATE)

2.  Average treatment effect on the treated (ATT)

3.  
