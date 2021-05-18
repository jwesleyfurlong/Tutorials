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

**'Impact' is a causal (or treatment) effect**

The goal of this post is to describe some import concepts for the use of causal inference methods to evaluate social programs.

A program's 'impact' refers to its causal (or treatment) effect, which is the expected change in outcome due to the program (i.e., intervention, treatment) *when compared with a baseline condition.* This last phrase is important.

Consider the example of a clinical program for foster youth where trauma-informed cognitive behavioral therapy and EMDR (eye movement desensitization and reprocessing) are both used with clients. What is the impact of each therapeutic approach? How does the effect of EMDR compare to trauma-informed CBT? Should both be used? Does it depend on factors like age or level of trauma? Each of these questions reflects a type of causal estimate.

**Why not just pre-post test?**

By itself, a pre-post test cannot yield a causal estimate because it does not answer the question, "What would have occurred without the treatment?" The person may have improved without the treatment. Many factors may influence pre-post scores.

![](simple_difference.png)

To answer causal questions, we need to know the difference for the child *with and without the treatment.* We need to distinguish two potential outcomes for the same person: when treated - when untreated.

Of course, it's impossible to identify more than one outcome for a single person.

> **Impact = factual- counterfactual**

'What happened' - 'what would've happened without the intervention'

Since counterfactuals aren't observable for specific individuals, we use a 'potential outcomes framework' to estimate causal effects on a program level.

![](counterfactual.png)

**Impact = causal effect = treatment effect**

The gold standard is a randomized controlled trial where, providing the assumptions are met, the average treatment effect is simply the difference between the treated and controlled group.

When we work with observational data where individuals are not randomly selected and placed into treatment and control, we aim to model experimental conditions to ensure treatment effects are not 'confounded' by any pre-treatment characteristics or spillover effects during treatment. How do you model randomization?

One way to address potential selection bias from a non-randomized sample is by carefully creating the control and treated groups with propensity scores, which estimate the probability of treatment given pre-treatment characteristics. This creates balance between the groups and hopefully gets us close to observing the unobservable- the two potential outcomes for 'close-to-the-same' person.

In future posts, we will dive deeper into propensity scores and the various methods for calculating them. For now, I want to distinguish three relevant types of causal effect estimates for program evaluation:

1.  Average treatment effect (ATE)

2.  Average treatment effect on the treated (ATT)

3.  Conditional average treatment effect (CATE)

**Average treatment effect:**

"How effective is the treatment for a randomly selected person in the population?"

The ATE is defined as the difference between treatment outcome and control outcome.

**Average treatment effect on the treated:**

"How would those who received the treatment had done if they hadn't received it?"

The ATT is the average benefit for those who received the treatment.

ATT is a helpful estimand when our target population is different from the population at large (e.g., children in foster care who are enrolled in a clinical program) and we want to estimate the difference between two interventions (e.g., trauma-informed CBT and EMDR).

**Conditional average treatment effects:**

The same treatment may affect individuals differently. CATE estimates the effect of treatment for different subgroups.

In the following posts, we will look at some program data and demonstrate methods for calculating causal estimates.
