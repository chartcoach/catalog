---
id: use-bar-charts-instead-of-pie-charts-for-ranking-part-sizes
title: Use a bar chart instead of a pie chart for ranking part sizes
bibliography: references.bib
description: For compare tasks, prefer bar charts over pie charts on part-to-whole
  quantitative categories to improve fidelity and mitigate angle-based ranking mistakes
  for readers making visual percentage judgments.
labels:
- purpose:select
- basis:empirical
- task:compare
- chart:bar:use
- chart:pie-donut:avoid
- quality:fidelity:use
- lever:chart-family
- operator:rank
---

## Bar instead of pie for ranking <!-- role: advice -->

Choose a bar chart when readers need to order or compare the sizes of parts. For example, use adjacent bars on a common baseline instead of pie slices when readers must judge which part is larger and how large the smaller part is relative to the larger.

## Why bar charts work better here <!-- role: reason -->

A shared linear scale makes part sizes easier to compare than slice angles. When readers need an ordered judgment rather than a decorative whole shape, bars let the eye compare values directly.

**Mechanism:** A common baseline turns the read into position judgments, which are more accurate here than angle judgments.

**Evidence:** In the reported sort experiment, the adjacent bar chart outperformed the pie chart for accuracy, and that difference was significant under the paper's bootstrap analysis; the collated record preserves this result as the recommended outcome for the sort task [@zengReviewCollationGraphical2023; @clevelandGraphicalPerceptionTheory1984].

## Use when the chart must support accurate part comparison <!-- role: context -->

- **User Goal:** Order parts and compare their sizes.
- **Task:** Rank quantitative parts and estimate one part relative to another.
- **Data:** Part-to-whole categories expressed as numeric amounts or percentages.
- **Chart Setting:** You are choosing between a pie chart and a one-series bar chart.
- **Audience:** Readers making quick visual judgments.
- **Success Criterion:** More accurate ordering and relative-size estimates.

## Do not use when the task is not magnitude comparison <!-- role: exceptions -->

**Break it when:** The graphic's main job is not to compare or rank magnitudes. **Why:** The reported evidence here is specific to sort judgments about quantitative values.

## What you give up by replacing the pie <!-- role: costs -->

**Sacrifice:** You lose the circular part-to-whole form.
**Risk:** Readers may lose an immediate sense that the values sum to a whole.
**Mitigation:** Use a simple whole-based bar scale, such as percentages from 0 to 100, when the whole reference matters.

## Common replacement mistake <!-- role: mistakes -->

**Mistake:** Replacing the pie chart with a divided or stacked bar that still forces readers to compare segment lengths. **Why it fails:** The same study found ordinary adjacent bars more accurate than stacked length-based variants.

## How to check the choice <!-- role: check -->

**Failure Sign:** Readers must compare slice angles to decide the order of parts.
**Quick Check:** Make a bar-chart version with one bar per part on a shared baseline and see whether the order becomes visually immediate.
**Stronger Test:** Ask a reviewer to identify the larger of two parts and estimate the smaller as a percentage of the larger in both versions.

## What to change <!-- role: fix -->

- Replace the pie slices with one bar per part on a common baseline.
- Use a whole-based bar scale when the chart still needs to communicate fractions of a whole.
- If the current replacement is segmented or stacked, unstack the values readers need to compare.
