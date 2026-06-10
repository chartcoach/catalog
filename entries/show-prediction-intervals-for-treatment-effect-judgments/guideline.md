---
id: show-prediction-intervals-for-treatment-effect-judgments
title: Show prediction intervals instead of confidence intervals for treatment-effect
  judgments
bibliography: references.bib
description: For individual-level treatment-effect judgments in experimental results,
  prefer outcome-uncertainty interval encoding on mean-with-interval charts to improve
  fidelity and mitigate overestimation of treatment effectiveness for lay readers.
labels:
- purpose:refine
- basis:empirical
- task:compare
- quality:fidelity:use
- lever:encoding
- operator:uncertainty
- audience:general-public
---

## Encode individual outcome variation <!-- role: advice -->

Encode outcome uncertainty directly when readers need to judge how effective a treatment will be for individuals. For example, replace 95% confidence-interval bars with 95% prediction-interval bars, or use intervals based on standard deviations rather than standard errors, on the same mean plot.

## Why prediction intervals work here <!-- role: reason -->

Confidence intervals visualize uncertainty in the estimated mean, while prediction intervals visualize the spread of individual outcomes. When readers use the chart to judge what will happen to them rather than what is known about the mean, narrow confidence intervals make the treatment look more effective and more reliable than it is.

**Mechanism:** Showing outcome uncertainty lets readers see how much the treatment and control distributions overlap, which improves judgments about treatment effectiveness, probability of superiority, and likely outcome variability.

**Evidence:** Across two preregistered experiments, plots with 95% confidence intervals led people to overstate willingness to pay, overstate probability of superiority, and understate outcome variability relative to plots with 95% prediction intervals built from the same underlying data [@hofmanHowVisualizingInferential2020].

**Notes:** The distortion was largest for smaller underlying effects.

## Use when all of these are true <!-- role: context -->

- **User Goal:** Decide whether a treatment or intervention is worth choosing.
- **Task:** Compare likely individual outcomes between two conditions.
- **Data:** Experimental results summarized as group means with interval bars.
- **Chart Setting:** A static plot shows one uncertainty encoding for each group.
- **Audience:** Lay readers or other nonexpert consumers of the result.
- **Success Criterion:** Readers estimate treatment advantage and outcome spread close to the underlying distributions.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** The chart's main job is to communicate inferential uncertainty about the mean or support significance-oriented reading rather than judgments about likely individual outcomes. **Why:** Confidence intervals directly encode mean-estimation uncertainty, and replacing them with outcome-uncertainty intervals can hide that information.

## Tradeoffs of prediction intervals <!-- role: costs -->

**Sacrifice:** You give up the most direct visual cue about uncertainty in the estimated mean.
**Risk:** Readers may have less support for significance-oriented reading from the figure alone.
**Mitigation:** Report inferential uncertainty elsewhere in the study if it also matters.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep 95% confidence-interval bars and assume readers will mentally convert them into outcome variability. **Why it fails:** Estimating individual-outcome spread from a confidence interval requires extra statistical conversion, and readers instead perceive a larger and more certain treatment effect.

## Review before publishing <!-- role: check -->

**Failure Sign:** The interval bars are very narrow and the treatment looks close to certain to help.
**Quick Check:** Ask whether the bars represent uncertainty in the mean or variation in individual outcomes; if they only represent mean uncertainty, they do not support individual-outcome judgments well.
**Stronger Test:** Build a 95% prediction-interval version of the same plot and compare the apparent treatment advantage; if the confidence-interval version makes the effect look materially larger, keep the prediction-interval version.

## Revise the chart <!-- role: fix -->

- Replace 95% confidence-interval bars with 95% prediction-interval bars.
- Compute the displayed interval from standard deviations rather than standard errors when the goal is to show variation in individual outcomes.
- Rewrite the caption so it describes variation in individual outcomes around each mean.
