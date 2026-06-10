---
id: use-scatterplot-over-positive-parallel-coordinates-for-correlation
title: Use a scatterplot instead of a positive parallel coordinates plot for correlation
  judgments
bibliography: references.bib
description: For relate tasks, use a scatterplot on bivariate quantitative correlation
  displays instead of a parallel coordinates plot to improve fidelity and mitigate
  imprecise positive-correlation judgments for readers distinguishing nearby association
  strengths.
labels:
- purpose:select
- basis:empirical
- task:relate
- chart:scatter:use
- chart:parallel:avoid
- data:quantitative
- quality:fidelity:use
- lever:chart-family
- operator:association
---

## Choose scatterplots over positive parallel coordinates <!-- role: advice -->

Use a scatterplot rather than a positive parallel coordinates plot when readers need to judge the strength of correlation between two quantitative variables. For example, if the same bivariate data can be shown as points in x/y position or as lines across two parallel axes, keep the scatterplot and avoid the positive parallel-coordinates version.

## Why the scatterplot works better here <!-- role: reason -->

This contrast is about precision, not stylistic preference. The better chart is the one that lets readers tell apart nearby correlation strengths more reliably.

**Mechanism:** The scatterplot produced smaller just-noticeable differences for positive correlations, so nearby positive association levels were easier to distinguish.

**Evidence:** Positive scatterplots significantly outperformed positive parallel coordinates in the correlation-judgment experiment, while negative parallel coordinates were not significantly different from scatterplots; the 2023 review collated this as an empirical relate-task finding [@harrisonRankingVisualizationsCorrelation2014; @zengReviewCollationGraphical2023].

## Use when positive association is the reading task <!-- role: context -->

- **User Goal:** Judge which of two displays shows the stronger positive correlation.
- **Task:** Compare nearby association strengths.
- **Data:** Two quantitative variables with positive correlation.
- **Chart Setting:** A single static view where scatterplot and parallel-coordinates versions are both feasible.
- **Success Criterion:** More reliable discrimination of nearby positive correlation values.

## Do not use this contrast when the parallel view can be made negative <!-- role: exceptions -->

**Break it when:** The parallel-coordinates version can be arranged so the same relationship appears as a negative correlation pattern. **Why:** Negative parallel coordinates performed comparably to scatterplots, while the positive parallel-coordinates version did not.

## What you give up by replacing the parallel view <!-- role: costs -->

**Sacrifice:** You give up the parallel-coordinates encoding for this judgment task.
**Risk:** If a parallel-coordinates view is required elsewhere in the workflow, replacing it may not fit the surrounding display.
**Mitigation:** If the parallel-coordinates form must stay, switch to a negative-correlation arrangement instead of keeping the positive one.

## Common chart-choice mistake <!-- role: mistakes -->

**Mistake:** Treating positive and negative parallel-coordinates layouts as equivalent for correlation judgment. **Why it fails:** The study found a clear asymmetry between them.

## How to test the choice <!-- role: check -->

**Failure Sign:** Readers struggle to tell which of two nearby positive correlations is stronger in the parallel-coordinates view.
**Quick Check:** Render the same positive-correlation data as a scatterplot and as a positive parallel-coordinates plot at the same size, then ask reviewers which of two close-correlation pairs is more correlated.
**Stronger Test:** Repeat that side-by-side judgment across several nearby correlation levels and keep the chart that produces more consistent answers.

## What to change <!-- role: fix -->

- Replace the positive parallel-coordinates view with a scatterplot for the correlation-reading step.
- Keep size, data, and correlation level matched when comparing the two versions.
- If the parallel-coordinates form must remain, flip or rearrange axes so the relationship appears as a negative pattern.
