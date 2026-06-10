---
id: mirror-bar-small-multiples-for-correlation
title: Mirror bar small multiples for correlation comparison
bibliography: references.bib
description: For comparison of similarity between two quantitative series in paired
  bar charts, prefer mirrored small-multiple alignment to improve fidelity and mitigate
  cross-panel correspondence errors for viewers judging which pair is more correlated.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:bar
- structure:small-multiples
- lever:layout-structure
- operator:association
- group-cardinality:binary
---

## Mirrored bar pairs for similarity <!-- role: advice -->

Mirror each pair of bar charts when viewers need to decide which pair is more similar or correlated. For example, center-align the two series and reverse one x-axis instead of keeping both charts in a standard adjacent left-to-right pair.

## Why mirrored bar small multiples work for this task <!-- role: reason -->

Correlation judgments depend on matching corresponding values across the pair, and mirror symmetry makes those matches easier to read.

**Mechanism:** Centered mirror alignment reduces cross-panel matching effort and supports faster, more precise comparison of overall similarity.

**Evidence:** In the bar-chart correlation experiment, mirrored small multiples let participants succeed at a lower target correlation than adjacent small multiples, and the paper reports no benefit for animation in this task [@ondovFaceFaceEvaluating2019].

## Use when all of these are true <!-- role: context -->

- **User Goal:** Decide which bar-chart pair is more similar or more correlated.
- **Task:** Compare pairs of bar-chart series rather than single values.
- **Data:** Two quantitative series per pair, with comparable means and standard deviations.
- **Chart Setting:** A static small-multiple bar layout is being used for a two-way comparison.
- **Audience:** Viewers inspect one paired comparison at a time.
- **Success Criterion:** Readers can distinguish higher from lower correlation at smaller correlation differences.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** You must compare more than two datasets at once. **Why:** The paper notes that mirroring implies only two datasets and is unlikely to scale.

## Tradeoffs of mirrored bar pairs <!-- role: costs -->

**Sacrifice:** A conventional same-direction x-axis on both charts.
**Risk:** The mirrored view is less scalable for many simultaneous comparisons.
**Mitigation:** Use it for direct two-way correlation judgments only.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep a same-direction adjacent pair when the task is to judge overall similarity between two bar-chart series. **Why it fails:** It gives up the center-aligned mirror structure that improved correlation comparison.

## How to test this choice <!-- role: check -->

**Failure Sign:** Readers need very high similarity before they can reliably pick the more correlated pair.
**Quick Check:** Show mirrored and standard adjacent versions of the same bar-chart pairs, then ask readers which pair is more similar.
**Stronger Test:** Reduce the correlation gap between the candidate pairs and keep the layout that still produces correct choices.

## What to change <!-- role: fix -->

- Reverse the x-axis direction of one chart in each pair.
- Center-align the two charts so corresponding bars face each other.
- Keep the mirrored view limited to two-way comparisons.
- If you must show many datasets at once, move back to a non-mirrored layout.
