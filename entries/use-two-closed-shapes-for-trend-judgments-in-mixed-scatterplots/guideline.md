---
id: use-two-closed-shapes-for-trend-judgments-in-mixed-scatterplots
title: Use two closed shapes for trend judgments in mixed scatterplots
bibliography: references.bib
description: For trend judgments in single-view scatterplots, prefer closed shape
  encodings on heterogeneous point displays to improve fidelity and mitigate slower
  or less accurate reading in mixed-symbol views for readers making rapid visual analytic
  judgments.
labels:
- purpose:refine
- basis:empirical
- task:trend
- chart:scatter
- quality:fidelity
- lever:encoding
- channel:shape:use
- density:dense
---

## Closed shape pairs <!-- role: advice -->

Use two closed shapes when one scatterplot must support trend judgments across two shape-coded groups. For example, replace an open-open pair such as asterisk plus cross with a closed-closed pair such as triangle plus square when both groups occupy the same mixed point cloud.

## Why closed pairs work for trend reading <!-- role: reason -->

Closed shapes are separated more efficiently than open line-based shapes when both groups share one dense field of points. That makes it easier to decide which group forms the clearer linear pattern.

**Mechanism:** Closed shapes reduce interference during mixed-symbol trend reading, so readers can identify the more linear group faster and with fewer mistakes.

**Evidence:** In the collated results, the closed-closed triangle-square pair ranked first for both accuracy and time on the correlate task, while the open-open asterisk-cross pair ranked last; the reported significant pairwise difference was closed-closed over open-open. The source paper also reports faster and more accurate processing for closed than open shapes and a closed-target advantage in single-plot linear-relationship judgments [@zengReviewCollationGraphical2023; @burlinsonOpenVsClosed2018].

**Notes:** The advantage depends on task and on whether both groups are mixed into one plot.

## Use when all are true <!-- role: context -->

- **User Goal:** Decide which of two groups shows the stronger linear relationship.
- **Task:** Trend judgment across two shape-coded groups.
- **Data:** Two quantitative axes with one categorical grouping mapped to shape.
- **Chart Setting:** One scatterplot contains both groups at once, and the point field is visually dense or cluttered.
- **Audience:** Readers making quick visual analytic judgments.
- **Success Criterion:** Higher trend-reading accuracy with shorter response time.

## Do not use when any are true <!-- role: exceptions -->

**Break it when:** The groups are shown in separate homogeneous plots, or the primary task is average-value judgment rather than trend judgment. **Why:** The study did not find a reliable open/closed advantage in side-by-side homogeneous displays, and the average-value task showed no significant shape-category effect.

## What this costs <!-- role: costs -->

**Sacrifice:** The rule is task-specific rather than a universal ranking for every scatterplot task.\
**Risk:** The benefit can weaken or change with difficulty and with the distractor category paired against the target.\
**Mitigation:** Validate the closed-closed mapping on the actual mixed-plot trend task instead of assuming it will transfer to other tasks.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep two open shapes in the same mixed scatterplot when the chart's job is trend judgment. **Why it fails:** The open-open pair was the worst trend condition, and open shapes were slower and less accurate to process than closed shapes.

## How to test it <!-- role: check -->

**Failure Sign:** Reviewers hesitate or disagree about which group forms the clearer line.\
**Quick Check:** If both legend symbols are open line-segment shapes in one mixed scatterplot, flag the chart for revision.\
**Stronger Test:** Compare the current mapping against a triangle-square version on the same data with a short timed trend-judgment check.

## What to change <!-- role: fix -->

- Replace the two open symbols with two closed symbols.
- Start with a triangle and square if you need a direct source-tested pair.
- If your chart already uses separate homogeneous plots, do not spend revision time on open-versus-closed pairing for this task.
