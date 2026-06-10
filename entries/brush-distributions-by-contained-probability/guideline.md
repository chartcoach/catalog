---
id: brush-distributions-by-contained-probability
title: Select uncertain values by contained probability, not by mean position
bibliography: references.bib
description: For interactive exploration of uncertain multivariate data, use probability-based
  brushing on scatter and parallel plots to improve trust and address mistaken selection
  of low-confidence samples for viewers working with statistically modeled uncertainty.
labels:
- purpose:refine
- basis:empirical
- chart:scatter
- chart:parallel
- lever:interaction-access
- operator:uncertainty
- quality:trust
---

## Probability-based brushing <!-- role: advice -->

Integrate each sample's distribution inside the brush and select it only when the enclosed probability mass exceeds a chosen threshold. For example, evaluate boxes, axis intervals, or line-based brushes against the distribution area and require a high containment threshold such as 95% so broad uncertain values need a larger brush than tight certain ones.

## Why probability-based brushing works <!-- role: reason -->

Brushing uncertain data should respect the same uncertainty model used in the rendering. Probability-based brushing prevents a tiny brush from selecting a broad uncertain sample just because its mean happens to lie inside.

**Mechanism:** The brush selects distributions rather than points. A selection succeeds only when most of the distribution is actually contained, which forces the interaction to acknowledge uncertainty magnitude.

**Evidence:** The paper extends brushing for uncertain scatter plots and parallel coordinates by integrating each distribution within the brush and recommends a high confidence threshold, such as 95%, so uncertain values require larger brushes before they are selected [@fengMatchingVisualSaliency2010].

## When to use probability-based brushing <!-- role: context -->

- **User Goal:** Interactively select uncertain values without overclaiming what the brush contains.
- **Task:** Filter or inspect uncertain samples with box, interval, angular, or linear-function brushes.
- **Data:** Samples represented as statistical distributions, including normal distributions with known parameters.
- **Chart Setting:** Interactive scatter plots or parallel coordinates of uncertain data.
- **Audience:** Analysts or domain experts exploring uncertain multivariate relationships.
- **Success Criterion:** Selected items are mostly contained within the brush according to their distributions, not just by mean location.

## When probability-based brushing fails <!-- role: exceptions -->

**Break it when:** The data are treated as exact discrete samples or no distribution or PDF is available to integrate. **Why:** There is no probability mass to evaluate against the brush.

## Tradeoffs of probability-based brushing <!-- role: costs -->

**Sacrifice:** Small quick brushes no longer select broad uncertain values.
**Risk:** Users may think the brush is unresponsive when it correctly rejects high-uncertainty samples.
**Mitigation:** Increase the brush size until it encloses the desired fraction of the selected distributions.

## Common mistake with probability-based brushing <!-- role: mistakes -->

**Mistake:** Select by testing whether a sample mean or line center falls inside the brush. **Why it fails:** A small brush can capture highly uncertain distributions even when most of their probability mass lies outside.

## How to check probability-based brushing <!-- role: check -->

**Failure Sign:** A small brush selects broad uncertain values that visibly extend far outside the brushed region.
**Quick Check:** Inspect any selected uncertain item and confirm that most of its distribution lies inside the brush.
**Stronger Test:** Verify that every selected item passes the same integrated-area threshold, such as 95%.

## How to fix probability-based brushing <!-- role: fix -->

- Replace inside-outside tests on means with integration of the distribution over the brushed region.
- For line-based brushes, integrate the distribution between bounding lines instead of checking only distance to a centerline.
- Raise the selection threshold so the brush must contain most of each selected distribution.
- Enlarge the brush when you intentionally want to include broad uncertain values.
