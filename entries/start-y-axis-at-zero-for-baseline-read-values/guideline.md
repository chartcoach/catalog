---
id: start-y-axis-at-zero-for-baseline-read-values
title: Start the y-axis at zero when values are read from the baseline
bibliography: references.bib
description: For at-a-glance magnitude comparison, use a zero y-axis on charts where
  values are read from the baseline to improve fidelity and mitigate exaggerated differences
  for readers relying on visual gist.
labels:
- purpose:refine
- basis:empirical
- task:compare
- quality:fidelity
- lever:scale-order
- operator:difference
- reading-mode:overview
- component:axis:use
---

## Zero baseline <!-- role: advice -->

Start the y-axis at zero when readers judge values by the distance from the x-axis. For example, in a bar chart or other baseline-read view, extend the axis to zero instead of truncating it above the data range.

## Why truncated baselines mislead <!-- role: reason -->

Readers form the gist of a chart before they read axis labels. When the baseline is moved upward, the visible distances between marks no longer match the numeric differences in the data.

**Mechanism:** A zero baseline keeps apparent size and apparent difference closer to the real values readers are trying to compare. This reduces exaggerated ratios that arise from truncated axes.

**Evidence:** The paper shows that non-zero y-axes can make small differences look much larger than they are, and it notes that people seldom read axis labels before drawing conclusions from what they see at a glance [@szafirGoodBadBiased2018].

## Use when readers compare magnitudes from the axis <!-- role: context -->

- **User Goal:** Compare magnitudes or differences quickly.
- **Task:** Judge relative size from mark height or position measured from the x-axis.
- **Data:** Quantitative values where raw magnitude matters.
- **Chart Setting:** A chart uses an axis and readers are expected to interpret it at a glance.
- **Audience:** Readers who will infer differences visually before reading labels closely.
- **Success Criterion:** Apparent ratios and differences match the actual data more closely.

## Do not use when the task is small variation in a line graph <!-- role: exceptions -->

**Break it when:** The chart is a line graph and the analysis cares about variation rather than magnitude. **Why:** The source notes this as a debated case because a zero baseline can make small variations hard to notice when variation is the quantity of interest.

## What you trade away <!-- role: costs -->

**Sacrifice:** You give up vertical space that could magnify small changes.
**Risk:** Important small-scale variation can become hard to see.
**Mitigation:** Compute and visualize change relative to a baseline, or visualize rate of growth, instead of truncating the raw axis.

## Common axis failure <!-- role: mistakes -->

**Mistake:** Truncating the y-axis and relying on labels to prevent misreading. **Why it fails:** Readers often see the apparent ratio first and never correct it with the labels.

## How to review the baseline <!-- role: check -->

**Failure Sign:** A modest numeric change looks like a dramatic visual jump.
**Quick Check:** Compare the visible ratio of mark heights to the numeric ratio in the data.
**Stronger Test:** Ask whether the chart suggests a much larger difference when viewed briefly than the numbers actually support.

## What to change <!-- role: fix -->

- Extend the y-axis to zero.
- Replot the same values with the zero baseline and compare the apparent ratio.
- If the story is about change from a baseline, compute that change and plot it directly.
- If the story is about growth or decline, plot the growth rate instead of truncating the raw values.
