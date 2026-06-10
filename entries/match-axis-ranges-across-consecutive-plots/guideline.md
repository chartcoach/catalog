---
id: match-axis-ranges-across-consecutive-plots
title: Use the same axis range across consecutive plots of the same variables
bibliography: references.bib
description: For comparison across repeated views of the same variables, use matching
  axis ranges on consecutive plots to improve fidelity and mitigate false crossings
  for readers comparing patterns across views.
labels:
- purpose:refine
- basis:empirical
- task:compare
- structure:multi-view
- quality:fidelity
- lever:scale-order
- operator:difference
- component:axis:use
---

## Matched axis ranges <!-- role: advice -->

Use the same axis range across consecutive plots that show the same variables. For example, if two adjacent charts both show the same service count or the same measure over time, keep their axes on the same scale instead of normalizing each plot separately.

## Why unequal scales create false stories <!-- role: reason -->

Readers compare chart shape and crossings visually. When each view uses a different axis range, the shapes change even though the underlying quantities did not.

**Mechanism:** Matching axis ranges preserves the visual meaning of slopes, gaps, and crossings across views. This prevents separate panels from implying changes that come only from renormalization.

**Evidence:** The paper warns that normalizing consecutive plots of the same variables to different ranges can create false crossings and misleading stories, while renormalizing them to the same scale changes the conclusion [@szafirGoodBadBiased2018].

## Use when multiple views invite direct comparison <!-- role: context -->

- **User Goal:** Compare patterns, crossings, or dominance across repeated views.
- **Task:** Compare the same variables across consecutive plots.
- **Data:** The same measured variables appear in more than one plot.
- **Chart Setting:** Plots are shown consecutively or side by side.
- **Audience:** Readers are expected to compare the views directly.
- **Success Criterion:** Visual patterns remain comparable across plots without scale-induced distortion.

## Do not use when the variables are not the same <!-- role: exceptions -->

**Break it when:** The plots do not show the same variables and are not meant for direct visual comparison. **Why:** The rule is tied to repeated views of the same quantities.

## What you trade away <!-- role: costs -->

**Sacrifice:** You give up per-plot scaling that maximizes the space devoted to each plot’s local data range.
**Risk:** A narrow-range panel can look visually compressed.
**Mitigation:** Keep the shared scale when cross-view comparison is the primary task.

## Common multi-view failure <!-- role: mistakes -->

**Mistake:** Fitting each plot to its own minimum and maximum while expecting readers to compare them directly. **Why it fails:** The changing scale can manufacture crossings or apparent reversals that are not in the data.

## How to review repeated scales <!-- role: check -->

**Failure Sign:** A crossing, reversal, or sharp pattern shift appears only because one panel uses a different range.
**Quick Check:** Read the minimum and maximum on each axis and verify they match.
**Stronger Test:** Replot the views on a common scale and see whether the main visual story changes.

## What to change <!-- role: fix -->

- Set identical axis limits across the consecutive plots.
- Replot all repeated views with the same range before comparing them.
- Remove per-panel normalization when the goal is cross-view comparison.
- Recheck any apparent crossing after the scales are matched.
