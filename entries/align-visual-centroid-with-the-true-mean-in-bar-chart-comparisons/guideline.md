---
id: align-visual-centroid-with-the-true-mean-in-bar-chart-comparisons
title: Align visual centroid with the true mean in bar-chart comparisons
bibliography: references.bib
description: For quick compare tasks, prefer centroid-aligned encoding on paired bar
  charts to improve fidelity and mitigate wrong larger-mean judgments for viewers
  making rapid perceptual comparisons.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:bar
- structure:multi-view
- quality:fidelity:use
- lever:encoding
- reading-mode:overview
---

## Centroid alignment <!-- role: advice -->

Align the occupied bar area so the chart with the larger arithmetic mean also has the more right-shifted visual center of mass. For example, avoid a smaller-mean bar chart whose long bars are pushed toward the high-value side or toward the extrema, because those patterns made it more likely to be chosen as having the larger mean.

## Why centroid alignment works <!-- role: reason -->

Quick mean judgments can follow a center-of-mass shortcut instead of an arithmetic calculation. When the smaller-mean chart visually places more bar area farther along the value axis, that shortcut can overpower the true answer.

**Mechanism:** Viewers can use the chart’s centroid-like impression as a proxy for mean, so a lower-mean series can look larger if its visual mass is shifted farther toward larger values.

**Evidence:** In the theory-driven experiment, centroid was the strongest misleading proxy on average for larger-mean judgments in paired bar charts. In the data-driven experiment, optimized deceptive charts for mean often pushed bars toward the extrema in ways consistent with centroid and hull-area motifs [@ondovRevealingPerceptualProxies2021].

**Notes:** The paper reports that proxy use varies across people, so centroid alignment reduces a common risk rather than guaranteeing correct judgments for every viewer.

## When centroid alignment applies <!-- role: context -->

- **User Goal:** Help viewers pick which of two bar-chart series has the larger mean.
- **Task:** Rapid visual comparison after a brief glance.
- **Data:** Two quantitative series shown with the same number of bars.
- **Chart Setting:** Side-by-side bar charts where bar arrangement is under design control.
- **Audience:** Viewers making quick perceptual judgments rather than computing values.
- **Success Criterion:** Viewers choose the chart with the larger mean reliably.

## When not to use centroid alignment as a review rule <!-- role: exceptions -->

**Break it when:** The comparison is not a rapid larger-mean judgment between paired bar charts, or the bar arrangement is fixed by the data semantics. **Why:** The evidence is specific to quick mean comparison in paired bar charts, and the paper notes that proxies depend on task and data arrangement.

## Costs of centroid alignment <!-- role: costs -->

**Sacrifice:** Some bar arrangements or candidate chart pairings become unsuitable for fast mean comparison.
**Risk:** Fixing centroid alignment alone can still leave another misleading cue, such as hull area or max bar, pointing to the wrong chart.
**Mitigation:** Review more than one proxy-like cue before finalizing the comparison.

## Common centroid alignment mistake <!-- role: mistakes -->

**Mistake:** Leaving a smaller-mean chart with its visual mass shifted farther toward larger values and assuming the arithmetic mean will remain obvious. **Why it fails:** Under brief exposure, viewers can choose the centroid-favored chart instead of the true larger-mean chart.

## How to check centroid alignment <!-- role: check -->

**Failure Sign:** The lower-mean chart looks more right-weighted overall than the higher-mean chart.
**Quick Check:** Compare the apparent center of occupied bar area across the two charts; if the lower-mean chart appears farther along the value axis, flag it.
**Stronger Test:** Run a brief forced-choice A/B review and verify that viewers still pick the chart with the larger mean.

## How to fix centroid alignment problems <!-- role: fix -->

- Reorder the bars, when order is not semantically fixed, so the lower-mean series does not place more visual mass toward larger values.
- Remove or replace candidate arrangements in which one very long bar or an extrema-heavy pattern shifts the smaller-mean chart’s centroid past the larger-mean chart.
- Compare alternative bar arrangements and keep the version in which centroid-like cues and arithmetic mean point to the same chart.
