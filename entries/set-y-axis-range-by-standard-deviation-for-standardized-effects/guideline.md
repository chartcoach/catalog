---
id: set-y-axis-range-by-standard-deviation-for-standardized-effects
title: Set the y-axis range by standard deviation when showing standardized effect
  size
bibliography: references.bib
description: For effect-size comparison, use a standard-deviation-based y-axis range
  on quantitative charts of standardized outcomes to improve fidelity and mitigate
  overstatement from minimal axes and understatement from full-range axes for readers
  with novice chart literacy.
labels:
- purpose:refine
- basis:empirical
- task:compare
- data:quantitative
- quality:fidelity:use
- lever:scale-order
- component:axis:use
- literacy:novice
---

## Set the y-axis by standard deviation <!-- role: advice -->

Set the y-axis range as a function of the outcome standard deviation when the chart is meant to communicate standardized effect size. For example, center the axis on the grand mean and extend it about 0.5 to 1 standard deviation in each direction, aiming for a total range near 1.5 standard deviations instead of using the smallest visible range or the full possible scale.

## Why this axis range works <!-- role: reason -->

Readers judge effect magnitude partly from the visual size of the difference in the plot. A too-narrow axis makes small effects look large, while a too-wide axis makes meaningful effects look trivial.

**Mechanism:** A y-axis tied to standard deviation makes the visual size of the gap better match the conceptual size of the effect, so readers are more calibrated when deciding whether an effect is small, medium, or large.

**Evidence:** Across five experiments with 57 naïve college students, bar and line charts whose y-axis covered roughly 1 to 2 standard deviations produced better sensitivity to effect magnitude and less bias than charts using the minimum visible range or the full 0 to 100 range. The paper recommends centering the axis on the grand mean and aiming for about 1.5 standard deviations because tested variants in that range performed similarly well. [@wittGraphConstruction2019]

## Use when effect size is the message <!-- role: context -->

- **User Goal:** Communicate how big an effect is, not just whether values differ.
- **Task:** Readers must judge or compare effect magnitude from the chart.
- **Data:** The outcome is quantitative, and effect size is interpreted in standard deviation units.
- **Chart Setting:** The chart has a y-axis whose range can be adjusted; the paper tested bar charts, bar charts with error bars, and line charts.
- **Audience:** Readers are not assumed to be domain experts.
- **Success Criterion:** Readers classify effect size with higher sensitivity and lower bias.

## Do not use this as a fixed rule outside its tested scope <!-- role: exceptions -->

- **Break it when:** Standard deviation is unknown or is not the field's basis for interpreting effect size. **Why:** The recommendation is explicitly limited to fields where effect size is standardized by standard deviation.
- **Break it when:** A 1 to 2 standard deviation window would cut off error bars, hide unusually large effects, or force nonsensical values such as negative performance. **Why:** The source says the range must be widened enough to include these cases.

## What this choice costs <!-- role: costs -->

**Sacrifice:** You give up either the full possible measurement scale or the most zoomed-in view of the observed data.
**Risk:** Applying a fixed 1.5 standard deviation window blindly can clip uncertainty displays or unusual effects.
**Mitigation:** Widen the axis enough to include error bars and very large effects, and keep scales consistent across multiple graphs when cross-graph comparison matters.

## Common y-axis failures <!-- role: mistakes -->

- **Mistake:** Let software set the y-axis to the minimum range needed to show the data. **Why it fails:** It exaggerates small differences and biases readers toward judging effects as larger than they are.
- **Mistake:** Force the y-axis to the full possible range when the goal is to read effect size. **Why it fails:** It compresses visual differences and biases readers toward judging effects as smaller than they are.

## Check the axis against the data scale <!-- role: check -->

**Failure Sign:** The same difference looks dramatically inflated or flattened because the axis is either tightly cropped or stretched across the full measurement scale.
**Quick Check:** Compute the grand mean and standard deviation of the plotted outcome, then verify that the y-axis is roughly centered on that mean and spans about ±0.5 to ±1 standard deviation.
**Stronger Test:** Make an SD-based version of the chart and compare it with the current version; if the current axis is just the minimal visible span or the full possible span, replace it.

## Revise the y-axis range <!-- role: fix -->

- Recenter the y-axis on the grand mean of the plotted conditions.
- Reset the y-axis to about ±0.75 standard deviation, or within the tested range of ±0.5 to ±1 standard deviation.
- Expand the axis if needed so all error bars and unusually large effects remain visible.
- Widen the axis if the SD-based range would introduce nonsensical values or would prevent consistent comparison across related graphs.
