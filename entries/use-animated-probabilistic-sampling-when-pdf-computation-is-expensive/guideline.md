---
id: use-animated-probabilistic-sampling-when-pdf-computation-is-expensive
title: Use animated probabilistic sampling when full density computation is too expensive
bibliography: references.bib
description: For overview of very large uncertain multivariate data, use animated
  probabilistic sampling on scatter and parallel plots to improve insight and address
  hidden outliers for viewers scanning dense distributions.
labels:
- purpose:refine
- basis:empirical
- lever:encoding
- operator:uncertainty
- density:dense
- temporal-pattern:dynamic
- quality:insight
---

## Probabilistic sampling <!-- role: advice -->

Animate the plot by repeatedly drawing random samples from the underlying data PDF instead of waiting for a full density image. For example, resample points in a scatter plot or lines in parallel coordinates each frame so dense regions stay stable, rare outliers flicker in and out, and accumulated samples approximate the PDF.

## Why probabilistic sampling works <!-- role: reason -->

A single sampled frame is only a rough draw from the distribution, but animation turns repeated sampling into a useful summary. Stable regions reveal high density, and intermittent flicker calls attention to outliers that density summaries can hide.

**Mechanism:** Dense regions recur in many random samples and therefore appear stable over time. Sparse regions appear only occasionally, so outliers flicker. If samples are accumulated, the display converges toward a histogram approximation of the PDF.

**Evidence:** The paper introduces probabilistic plots for very large uncertain data, shows that animated random sampling keeps dense regions stable, makes outliers flicker, and demonstrates convergence toward the density plot as more sampled lines are accumulated [@fengMatchingVisualSaliency2010].

## When to use probabilistic sampling <!-- role: context -->

- **User Goal:** Get a fast overview of a very large uncertain data set and notice outliers.
- **Task:** Summarize dense uncertain structure when exact PDF computation is too slow.
- **Data:** Uncertain multivariate data with a samplable underlying PDF; in the paper, equal-weight records with independent normal per-variable distributions allow fast sampling.
- **Chart Setting:** Scatter plots or parallel coordinates where computing the full density image is expensive.
- **Audience:** Analysts or domain experts scanning large uncertain data.
- **Success Criterion:** Dense regions remain visually stable over time, sparse regions flicker, and accumulated samples approach the PDF.

## When probabilistic sampling fails <!-- role: exceptions -->

**Break it when:** A full density plot can already be computed interactively and the task needs an exact density summary immediately. **Why:** Probabilistic sampling is an approximation, and any single sampled frame can contain false patterns.

## Tradeoffs of probabilistic sampling <!-- role: costs -->

**Sacrifice:** You give up exact single-frame density for speed.
**Risk:** A static sample can misrepresent the underlying variability.
**Mitigation:** Keep the display animated or accumulate multiple sampled frames into a histogram buffer.

## Common mistake with probabilistic sampling <!-- role: mistakes -->

**Mistake:** Show one static random sample as the final summary. **Why it fails:** A single set of random samples may contain false patterns and does not accurately represent the full variability of the PDF.

## How to check probabilistic sampling <!-- role: check -->

**Failure Sign:** Dense regions drift wildly from frame to frame, or outliers never stand out as intermittent events.
**Quick Check:** Watch several frames and confirm that high-density regions persist while sparse regions appear only briefly.
**Stronger Test:** Accumulate successive samples into a histogram and confirm that the image moves toward the expected density pattern.

## How to fix probabilistic sampling <!-- role: fix -->

- Redraw new random samples continuously instead of freezing one sample set.
- Sample from the underlying data PDF rather than from screen space.
- Accumulate successive samples into a normalized histogram when you need a closer PDF approximation.
- Use the direct density plot once its computation becomes practical and exact density analysis matters more than speed.
