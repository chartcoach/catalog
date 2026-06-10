---
id: permute-colorfield-cells-within-known-intervals
title: Permute colorfield cells within known intervals for average judgments
bibliography: references.bib
description: For overview comparison of averages across predetermined intervals in
  ordered time series, use within-interval permutation on a colorfield display to
  improve judgment fidelity and address difficulty on close or noisy interval comparisons
  for viewers making aggregate assessments.
labels:
- purpose:refine
- basis:empirical
- task:compare
- time:ordered-time
- chart:heatmap
- quality:fidelity:use
- lever:layout-structure
- reading-mode:overview
---

## Permute the cells inside each interval block <!-- role: advice -->

Shuffle values within each known aggregation interval of a colorfield when the task is to compare interval averages. For example, randomly permute the colored cells inside each month block of a time-series colorfield so local color mixtures represent the block average more directly than the original ordered strip.

## Why within-interval permutation helps the colorfield <!-- role: reason -->

Within a colorfield, permutation brings the colors to be averaged closer together and makes smaller local regions look more like the interval as a whole. That improves average judgments for the color display, but the same idea did not help line graphs.

**Mechanism:** When color samples from the same interval are spatially mixed, viewers can pool more local color evidence instead of averaging across a longer ordered run.

**Evidence:** In the study, permuted colorfields outperformed ordered colorfields on the interval-average task, while permuting line graphs did not produce a significant benefit, yielding a significant interaction between display type and permutation [@correllComparingAveragesTime2012].

**Notes:** The paper treats this as a more specialized move than the base colorfield because it depends on known aggregation boundaries and removes low-level patterns within the interval.

## Use when the interval boundaries are fixed and known <!-- role: context -->

- **User Goal:** Choose which predefined interval has the highest average.
- **Task:** Compare averages across fixed interval blocks already shown in the display.
- **Data:** One ordered series encoded as color blocks, where preserving within-interval order is not required for the immediate task.
- **Chart Setting:** A colorfield or heatmap-like strip with explicit interval boundaries.
- **Audience:** Viewers making rapid aggregate judgments from the full display.
- **Success Criterion:** Higher accuracy on the interval-average decision than the ordered colorfield version.

## Do not permute when order inside the interval matters <!-- role: exceptions -->

**Break it when:** The aggregation duration is not known in advance, or readers need the within-interval temporal pattern. **Why:** The method depends on predefined aggregation ranges and the permutation destroys the original low-level ordering.

## Tradeoffs of permuting the colorfield <!-- role: costs -->

**Sacrifice:** You lose the original order and low-level pattern inside each interval.
**Risk:** The permuted block can show visual patterns that are not representative of the original sequence.
**Mitigation:** Limit the permutation to cases where fixed-interval average judgment matters more than within-interval sequence interpretation.

## Common failure mode: applying the same shuffle to a line chart <!-- role: mistakes -->

**Mistake:** Permuting points inside each interval of a line chart to improve average judgments. **Why it fails:** The study found no significant performance gain from permuted line graphs.

## How to test whether permutation helps <!-- role: check -->

**Failure Sign:** Readers still struggle to identify the best interval on an ordered colorfield, especially when top intervals are close or noisy.
**Quick Check:** Compare ordered and permuted versions of the same colorfield on representative hard cases and measure which one yields more correct interval choices.
**Stronger Test:** Include noisy series and close competing intervals, where the performance difference was most apparent.

## What to change <!-- role: fix -->

- Randomly permute the colorfield cells inside each predefined interval block.
- Keep the permutation confined within each interval so interval membership stays unchanged.
- Do not apply the same permutation as a repair for a line chart; use it only on the colorfield.
