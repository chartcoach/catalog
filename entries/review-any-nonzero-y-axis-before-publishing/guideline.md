---
id: review-any-nonzero-y-axis-before-publishing
title: Review any non-zero y-axis before publishing
bibliography: references.bib
description: For charts where readers should judge effect size without added emphasis,
  avoid non-zero y-axis baselines on bar and line charts to prevent exaggerated perceived
  effect size and address misleading severity judgments for readers interpreting how
  important a change feels.
labels:
- purpose:refine
- basis:empirical
- chart:bar
- chart:line
- lever:scale-order
- component:axis
- quality:fidelity:use
---

## Review the y-axis start <!-- role: advice -->

Avoid a non-zero y-axis start when you do not want the chart to make a change feel larger than the numbers justify. For example, compare any truncated bar chart or line chart against a 0-baseline version before publishing, because simply raising the y-axis start increased perceived severity in both chart types.

## Why the y-axis start changes the message <!-- role: reason -->

A higher y-axis start visually magnifies the same numeric gap. Readers then judge the change as more severe even when the underlying values stay the same, and that effect persists even when they can report the values accurately.

**Mechanism:** Truncation changes the apparent steepness or height contrast of the marks, so the chart communicates a stronger effect before the reader reasons through the numbers.

**Evidence:** Across three crowd-sourced experiments, higher y-axis starting points increased perceived severity in both bar charts and line charts, and the effect persisted even when participants estimated values accurately; the review paper collates this study as experimental evidence for visualization recommendation and critique workflows [@correllTruncatingYAxisThreat2020; @zengReviewCollationGraphical2023].

## Use when all are true <!-- role: context -->

- **User Goal:** Let readers judge how large or important a change feels without extra visual amplification.
- **Task:** Compare values or assess the strength of a trend.
- **Data:** Quantitative values on a vertical axis, often with a narrow dynamic range.
- **Chart Setting:** A static bar chart or line chart with a candidate non-zero y-axis start.
- **Success Criterion:** The chart's felt severity stays aligned with the numeric difference rather than with axis manipulation.

## Do not use when any are true <!-- role: exceptions -->

**Break it when:** The intended message is specifically about meaningful variation within a narrow non-zero range rather than about absolute magnitude from zero. **Why:** The paper argues there is no domain-agnostic truthful baseline, so the axis range can be chosen deliberately to match the effect size the chart is meant to communicate.

## Costs of changing the y-axis start <!-- role: costs -->

**Sacrifice:** Restoring a 0-baseline can compress small differences and make them less visually prominent.\
**Risk:** Applying a zero baseline automatically can hide a small but important change.\
**Mitigation:** Review both the 0-baseline and truncated versions, then keep the one whose emphasis matches the intended effect size.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Treating line charts as safe to truncate while treating bar charts as unsafe. **Why it fails:** The study found the same inflation pattern in perceived severity for both chart families.

## Check the effect of the axis choice <!-- role: check -->

**Failure Sign:** The same data feels much more dramatic after only the y-axis start changes.\
**Quick Check:** Put the truncated version next to a 0-baseline version and ask whether the numeric story stayed the same while the felt severity rose.\
**Stronger Test:** Ask a reviewer to rate how different or how fast-changing the series feels in both versions; if ratings rise with truncation, the axis choice is driving the message.

## Fix the axis decision <!-- role: fix -->

- Lower the y-axis start toward 0 when the stronger visual effect is not intended.
- Keep a truncated y-axis only when the intended comparison is variation within that narrower range.
- Review the chosen chart against a 0-baseline alternative before publishing.
- Treat the final y-axis range as an explicit framing decision, not as a neutral default.
