---
id: keep-standard-scatterplot-presets-for-correlation-estimation
title: Keep a standard scatterplot preset for correlation estimation
bibliography: references.bib
description: For relate tasks, avoid switching among tested scatterplot presets on
  quantitative scatterplots to prevent unsupported expectations of fidelity gains
  and address unnecessary preset churn in preset-selection workflows.
labels:
- purpose:refine
- basis:empirical
- task:relate
- chart:scatter
- data:quantitative
- quality:fidelity:use
- lever:encoding
---

## Scatterplot preset for correlation reading <!-- role: advice -->

Keep a standard scatterplot preset when the job is to judge correlation. For example, the evaluated task-tuned, package-default, and prior-study scatterplots showed no significant differences in correlation accuracy or completion time.

## Why preset switching does not help here <!-- role: reason -->

When tested presets perform equivalently on the same correlation-reading task, switching among them does not buy measurable performance. In that situation, extra preset tuning adds process without improving correlation judgments.

**Mechanism:** If accuracy and time stay unchanged across tested scatterplot presets, a standard preset is sufficient for the correlation-reading task being performed.

**Evidence:** In the collated extraction, the optimizer-generated, MATLAB, R, and prior-study scatterplots tied for both correlation accuracy and correlation time, with no significant pairwise differences [@micallefPerceptualOptimizationVisual2017; @zengReviewCollationGraphical2023].

**Notes:** This guideline is bounded to the tested scatterplot presets and the correlation-estimation task.

## Use when choosing among existing scatterplot presets <!-- role: context -->

- **User Goal:** Judge the correlation between two quantitative variables.
- **Task:** Correlation estimation.
- **Data:** Quantitative point data shown as a scatterplot.
- **Chart Setting:** You are choosing among already available scatterplot presets rather than changing chart family.
- **Success Criterion:** Correlation-reading accuracy and completion time are the deciding measures.

## Do not use when the task changes <!-- role: exceptions -->

**Break it when:** The task changes from correlation estimation to anomaly detection. **Why:** In this study, preset choice did matter for anomaly detection.

## Costs of keeping the standard preset <!-- role: costs -->

**Sacrifice:** You give up the possibility of an untested custom improvement.
**Risk:** You may overgeneralize this tie and assume preset choice never matters for other scatterplot tasks.
**Mitigation:** Apply this rule only when the decision is among similar tested presets for correlation estimation.

## Common over-tuning failure <!-- role: mistakes -->

**Mistake:** Retune or swap among tested scatterplot presets expecting measurable gains for correlation estimation. **Why it fails:** The tested presets did not differ in either correlation accuracy or completion time.

## Check whether preset switching is worth it <!-- role: check -->

**Failure Sign:** Teams keep changing scatterplot presets for correlation reading without measured performance gains.
**Quick Check:** Run an A/B comparison between the current preset and a standard preset on data with known correlation answers, and record both accuracy and completion time.
**Stronger Test:** If the presets tie on both measures, keep the standard preset.

## Fix unnecessary preset churn <!-- role: fix -->

- Revert to a standard scatterplot preset when correlation estimation is the only task.
- Stop switching among tested presets unless you can show a gain in correlation accuracy or completion time.
- Reserve extra preset tuning for tasks where the comparison shows a measurable difference.
