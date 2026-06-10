---
id: use-a-pie-chart-instead-of-a-treemap-for-few-slice-part-to-whole-comparisons
title: Use a pie chart instead of a treemap for few-slice part-to-whole comparisons
bibliography: references.bib
description: For exact part-to-whole comparison, prefer a pie chart over a treemap
  on few-category single-level share displays to improve fidelity and address higher
  percentage-estimation error for readers judging one segment at a time.
labels:
- purpose:select
- basis:empirical
- chart:pie-donut:use
- chart:treemap:avoid
- quality:fidelity:use
- lever:chart-family
- operator:part-whole
- group-cardinality:few
- reading-mode:exact
---

## Replace the chart family <!-- role: advice -->

Choose a pie chart instead of a treemap when the reader must estimate the share of one segment in a small part-to-whole display. For example, replace a single-level treemap of five shares with a pie chart when the task is to read one category's percentage of the whole.

## Why the pie chart works better here <!-- role: reason -->

The tested treemap made percentage judgments less precise than the tested pie chart in a few-segment part-to-whole display. This matters when the chart's job is to let readers estimate one segment's share rather than browse a packed rectangular layout.

**Mechanism:** The pie chart gave readers a more accurate visual basis for estimating one segment's fraction of the whole than the treemap in the tested five-segment displays.

**Evidence:** In the extracted experimental ranking for accuracy on the study's part-to-whole comparison task, the pie chart ranked above the treemap, and the recorded significance pairs show the pie chart as significantly more accurate than the treemap [@zengReviewCollationGraphical2023; @kosaraImpactDistributionChart2019].

**Notes:** The evidence is about accuracy, not a broad claim that pie charts are best for every part-to-whole design.

## Use when this situation is true <!-- role: context -->

- **User Goal:** Estimate how much of the whole a selected segment represents.
- **Task:** Read or compare segment percentages in a part-to-whole display.
- **Data:** One-level part-to-whole data with a few segments; the tested case used five segments.
- **Chart Setting:** Static single-view chart used for direct percentage reading.
- **Audience:** Readers answering direct percentage questions about a chosen segment.
- **Success Criterion:** Lower percentage-estimation error.

## Do not use when this condition breaks <!-- role: exceptions -->

**Break it when:** The display is not a few-segment, single-level part-to-whole chart or the task is not estimating a segment's share of the whole. **Why:** The evidence only covers five-segment part-to-whole judgments in this specific comparison.

## Costs of replacing the treemap <!-- role: costs -->

**Sacrifice:** You give up the treemap's rectangular packing and any value it has as a space-filling layout.
**Risk:** A pie chart is only supported here against a treemap, not as the best option against every other part-to-whole chart.
**Mitigation:** Use this replacement only for the tested use case: a few segments and direct percentage reading.

## Common mistake in this comparison <!-- role: mistakes -->

**Mistake:** Keeping a treemap as the default chart for a few-category part-to-whole readout. **Why it fails:** In the tested five-segment displays, the treemap produced higher percentage-estimation error than the pie chart.

## How to check the decision <!-- role: check -->

**Failure Sign:** Reviewers give less accurate percentage estimates from the treemap than from an equivalent pie chart.
**Quick Check:** Build matched pie and treemap versions with the same few shares and ask reviewers to estimate the same target segment in both versions.
**Stronger Test:** Run a timed A/B test on the same target-segment percentage questions and compare estimation error between the pie chart and treemap.

## What to change <!-- role: fix -->

- Replace the single-level treemap with a pie chart when the display shows only a few shares of one whole.
- Keep the same segment set across both versions so the revision changes chart family rather than content.
- Re-test the target percentage questions on the pie chart and keep the version with lower estimation error.
