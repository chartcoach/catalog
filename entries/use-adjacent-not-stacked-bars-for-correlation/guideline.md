---
id: use-adjacent-not-stacked-bars-for-correlation
title: Use adjacent rather than stacked bar pairs for correlation comparison
bibliography: references.bib
description: For comparison of similarity between two quantitative series in paired
  bar charts when using conventional small multiples, prefer adjacent placement over
  stacked placement to improve fidelity and mitigate cross-panel correspondence errors
  for viewers judging which pair is more correlated.
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

## Adjacent bar pairs for similarity <!-- role: advice -->

Place each bar-chart pair side by side rather than stacking the pair vertically when viewers compare similarity or correlation. For example, use left-right bar pairs instead of top-bottom bar pairs when asking which pair is more similar.

## Why adjacent bar pairs work better than stacked pairs here <!-- role: reason -->

For this task, side-by-side placement makes correspondence between paired bars easier than a vertical stack.

**Mechanism:** Adjacent placement shortens the comparison path between corresponding bars, while stacked placement makes viewers work harder to match values across the two panels.

**Evidence:** In the bar-chart correlation experiment, adjacent small multiples outperformed stacked small multiples, and mirrored small multiples improved further beyond adjacent [@ondovFaceFaceEvaluating2019].

## Use when all of these are true <!-- role: context -->

- **User Goal:** Decide which bar-chart pair is more similar or more correlated.
- **Task:** Compare pairs of quantitative bar-chart series.
- **Data:** Two quantitative series per pair, with comparable means and standard deviations.
- **Chart Setting:** You want a conventional same-direction small-multiple layout rather than a mirrored one.
- **Audience:** Viewers inspect one paired comparison at a time.
- **Success Criterion:** Readers can identify the more correlated pair without requiring very large correlation differences.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** You can use a mirrored two-way small-multiple pair instead. **Why:** The same experiment showed mirrored bar pairs were more precise than standard adjacent pairs.

## Tradeoffs of adjacent bar pairs <!-- role: costs -->

**Sacrifice:** The shared baseline alignment that stacked panels provide.
**Risk:** A conventional adjacent pair is still weaker than a mirrored pair for this task.
**Mitigation:** Use adjacent as the fallback when you want conventional same-direction axes.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Stack the two bar charts vertically and assume the common baseline will outweigh the harder cross-panel matching. **Why it fails:** The correlation task depends more on correspondence between the paired bars than on the stacked baseline.

## How to test this choice <!-- role: check -->

**Failure Sign:** Readers struggle more with top-bottom bar pairs than with left-right pairs on the same data.
**Quick Check:** Show the same correlated and less-correlated bar pairs once in adjacent form and once in stacked form, then ask readers which pair is more similar.
**Stronger Test:** Reduce the correlation gap and keep the placement that still yields correct choices.

## What to change <!-- role: fix -->

- Move the second chart beside the first instead of above or below it.
- Keep corresponding categories aligned across the left-right gap.
- If the adjacent pair is still hard to compare, reverse one axis and mirror the pair.
