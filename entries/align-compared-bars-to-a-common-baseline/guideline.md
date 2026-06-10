---
id: align-compared-bars-to-a-common-baseline
title: Align compared bars to a common baseline
bibliography: references.bib
description: For compare tasks, prefer position encoding on bar charts to improve
  fidelity and address errors from judging segment length without a shared baseline
  for readers making exact value judgments.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:bar
- data:quantitative
- quality:fidelity:use
- lever:encoding
- channel:position:use
- channel:length:avoid
- reading-mode:exact
---

## Common baseline alignment <!-- role: advice -->

Align the compared values to a common baseline so readers judge position rather than segment length. For example, use side-by-side bars or bottom-aligned segments instead of top segments in stacked bars or one segment placed on top of another.

## Why common-baseline bar comparisons work <!-- role: reason -->

A shared baseline turns the comparison into a direct read of position on one scale. Unequal starting points force readers to infer values from bar lengths, which increases error in quick proportional judgments.

**Mechanism:** Common-baseline placement lets readers compare where marks land on the same axis. Top-of-stack and stacked-on-top layouts remove that shared start point and make the comparison depend on length estimation.

**Evidence:** In the collated results, the common-scale bar variants ranked highest for accuracy. Under the reported 95% bootstrap test, the top two common-baseline variants significantly outperformed both top-segment and stacked-on-top length variants, and another common-scale variant significantly outperformed the stacked-on-top variant in proportional judgments [@zengReviewCollationGraphical2023; @heerCrowdsourcingGraphicalPerception2010].

## Use when exact bar comparisons matter <!-- role: context -->

- **User Goal:** Compare two marked quantitative values accurately.
- **Task:** Estimate how large one marked value is relative to another.
- **Data:** Quantitative values shown as bars or stacked bar segments.
- **Chart Setting:** The compared values currently sit in grouped bars, stacked bars, or another bar-like arrangement.
- **Audience:** Readers making quick visual judgments.
- **Success Criterion:** Higher accuracy in the comparison.

## Do not generalize beyond the tested comparison task <!-- role: exceptions -->

**Break it when:** The chart is not being used for an exact proportional comparison between marked bar values. **Why:** The evidence here only tests quick percentage judgments between marked values.

## Tradeoffs of re-aligning bars <!-- role: costs -->

**Sacrifice:** You may need to change a stacked arrangement or move compared segments out of their current positions.\
**Risk:** If you keep unequal starting points and only relabel the chart, readers still have to judge length.\
**Mitigation:** Move the compared values onto one baseline rather than leaving them at different heights.

## Common baseline mistakes <!-- role: mistakes -->

**Mistake:** Keeping the compared values at the tops of stacks or placing one compared bar directly on top of the other. **Why it fails:** The comparison still depends on length from different starting points, which was less accurate than common-scale position judgments.

## Check for unequal starting points <!-- role: check -->

**Failure Sign:** The two target values do not start from the same baseline.\
**Quick Check:** Trace each compared value back to where it starts on the axis; if the starts differ, the chart is asking for length comparison.\
**Stronger Test:** Mock up a shared-baseline version and see whether reviewers estimate the proportion more consistently.

## Fix the baseline <!-- role: fix -->

- Replot the compared values so they share one baseline on the same linear axis.
- Change top-segment comparisons into side-by-side or bottom-aligned comparisons.
- Move stacked-on-top comparisons onto a common scale before asking for an exact value judgment.
