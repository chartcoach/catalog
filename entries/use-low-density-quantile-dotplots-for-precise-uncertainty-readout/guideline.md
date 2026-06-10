---
id: use-low-density-quantile-dotplots-for-precise-uncertainty-readout
title: Use low-density quantile dotplots when viewers must estimate probabilities
  precisely
bibliography: references.bib
description: For exact probability-interval estimation in static timeline views of
  continuous predictive uncertainty, use low-density discrete-outcome encoding on
  timeline rows to improve fidelity and mitigate imprecise interval reading for novice
  mobile users.
labels:
- purpose:refine
- basis:empirical
- chart:timeline
- operator:uncertainty
- reading-mode:exact
- density:sparse
- quality:fidelity:use
- lever:encoding
- literacy:novice
---

## Low-density quantile dotplots <!-- role: advice -->

Encode predictive uncertainty with a small, countable set of evenly spaced quantile dots when users must estimate interval probabilities from a static view. For example, replace a static density plot with a quantile dotplot of about 20 dots on each timeline row so viewers can judge the chance that an event happens before a threshold by counting or quickly grouping dots.

## Why low-density quantile dotplots work <!-- role: reason -->

Low-density quantile dotplots turn a continuous predictive distribution into a small set of discrete outcomes that people can treat like frequencies. That makes interval judgments more concrete, especially near the tails, without requiring animated sampling or a large display.

**Mechanism:** A small number of dots lets viewers estimate risk by counting or subitizing small groups instead of inferring area from a smooth shape. This reduces response variability and supports better self-assessment of confidence.

**Evidence:** In the controlled experiment, the 20-dot quantile dotplot produced the lowest variance in probability estimates, about 1.15× more precise than the density plot, and also yielded the highest confidence; the 100-dot version performed similarly to density, and the stripeplot performed worse [@kayWhenIshMy2016].

**Notes:** The density plot was rated more visually appealing, so the precision gain comes with an aesthetic tradeoff.

## When to use low-density quantile dotplots <!-- role: context -->

- **User Goal:** Make a quick decision based on the chance that an event occurs before or within a time threshold.
- **Task:** Estimate a cumulative or interval probability from a predictive distribution.
- **Data:** Continuous predictive uncertainty for a single future event, often with skew.
- **Chart Setting:** Static small-screen timeline rows with limited space and little time for interaction.
- **Audience:** Everyday non-expert users with limited statistical training.
- **Success Criterion:** Probability estimates are more precise and users feel confident about them.

## When not to use low-density quantile dotplots <!-- role: exceptions -->

**Break it when:** Visual appeal is the primary success criterion and a small loss in estimation precision is acceptable. **Why:** The density plot was more visually appealing while being only slightly less precise.

## Tradeoffs of low-density quantile dotplots <!-- role: costs -->

**Sacrifice:** You give up some visual smoothness and some fine-grained density detail.
**Risk:** If you add too many dots, users stop reading the display as countable outcomes and the precision advantage disappears.
**Mitigation:** Keep the dot count low enough that the display still supports quick grouping and selective counting.

## Common mistakes with low-density quantile dotplots <!-- role: mistakes -->

**Mistake:** Packing the display with many dots or stripe-like marks. **Why it fails:** The display starts behaving like a continuous area or opacity encoding, so viewers no longer get the countability benefit.

## How to check low-density quantile dotplots <!-- role: check -->

**Failure Sign:** Users give widely scattered probability estimates or say they are judging the filled shape instead of the dot counts.
**Quick Check:** Show the same predictive scenario in your current density plot and in a low-density quantile dotplot, then ask several target users for the chance of arriving before a threshold; keep the version with tighter estimates and higher confidence.
**Stronger Test:** Inspect the stacks of dots; if vertical groups often exceed about five dots, the plot is too dense to support fast subitizing.

## How to fix low-density quantile dotplots <!-- role: fix -->

- Reduce the number of displayed outcomes to a small set, around 20 rather than 100.
- Space the dots so most vertical groups remain small enough to be quickly grouped.
- Replace stripe-like or very dense discrete encodings with a low-density quantile dotplot.
- Generate the dots from evenly spaced quantiles rather than random draws so the display is stable from one instance to the next.
