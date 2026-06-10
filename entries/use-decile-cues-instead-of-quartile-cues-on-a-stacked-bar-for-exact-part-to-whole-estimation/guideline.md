---
id: use-decile-cues-instead-of-quartile-cues-on-a-stacked-bar-for-exact-part-to-whole-estimation
title: Use decile cues instead of quartile cues on a stacked bar for exact part-to-whole
  estimation
bibliography: references.bib
description: For exact part-to-whole estimation, prefer decile internal cues over
  quartile internal cues on stacked bar charts to improve accuracy and address weak
  anchor placement for readers judging a highlighted share when no external scale
  is shown.
labels:
- purpose:refine
- basis:empirical
- chart:bar
- quality:fidelity:use
- lever:text-annotation
- operator:part-whole
- reading-mode:exact
- component:annotation:use
---

## Use denser internal cue marks on the bar chart <!-- role: advice -->

Use decile cues when you add internal reference marks to a stacked bar for exact part-to-whole estimation. For example, add tenth-interval cue marks inside the bar instead of quartile cue marks when you need anchors but cannot show an external scale.

## Why decile cues work better than quartile cues <!-- role: reason -->

This refinement changes the density of the internal reference marks while keeping the same bar-chart structure. In the tested cue variants, decile marks improved accuracy more than quartile marks.

**Mechanism:** Denser internal cue marks give readers more usable anchor points for estimating the highlighted share than quartile marks do.

**Evidence:** In the bar-cue comparison, the bar with decile cues ranked above both the bar with quartile cues and the baseline bar for accuracy, with significant differences reported against both; the quartile-cue bar was not reported as significantly better than baseline. The review records this as a within-bar refinement result from the collated study [@redmondVisualCuesEstimation2019; @zengReviewCollationGraphical2023].

## Use when internal anchors are the available refinement <!-- role: context -->

- **User Goal:** Improve exact estimation while keeping the stacked bar chart.
- **Data:** Two segments that sum to 100%.
- **Chart Setting:** No external quantitative scale is shown, but internal cue marks can be added.
- **Success Criterion:** Lower absolute error than the baseline bar or a quartile-cue bar.

## Do not use when a scale can be shown instead <!-- role: exceptions -->

**Break it when:** The chart can accommodate an external quantitative scale. **Why:** The source found the scaled bar more accurate than the decile-cue bar.

## Costs of using denser cue marks <!-- role: costs -->

**Sacrifice:** You add more internal marks than the quartile-cue version.
**Risk:** Stopping at quartile cues can leave the bar close to baseline performance instead of delivering the stronger gain seen with decile cues.
**Mitigation:** If the chart must use internal anchors, prefer deciles; if space allows, add an external scale instead.

## Common cue-mark mistake <!-- role: mistakes -->

**Mistake:** Add quartile cues and assume any internal anchor pattern will help enough. **Why it fails:** In the tested bar refinements, decile cues outperformed quartile cues, while quartile cues did not show a significant improvement over the baseline bar.

## Check the cue density directly <!-- role: check -->

**Failure Sign:** Readers still misjudge the highlighted share after internal cues are added.
**Quick Check:** Compare the same stacked bar with quartile cues and with decile cues, then ask reviewers to estimate the highlighted share as a whole number.
**Stronger Test:** Compare both cue versions against the baseline bar to confirm that the denser cue pattern is the version reducing error.

## Fix the cue marks <!-- role: fix -->

- Replace quartile cue marks with decile cue marks inside the stacked bar.
- Keep the bar segments unchanged so the cue density is the only revision.
- If the chart can support it, replace internal cue marks with an external quantitative scale.
