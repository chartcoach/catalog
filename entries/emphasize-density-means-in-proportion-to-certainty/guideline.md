---
id: emphasize-density-means-in-proportion-to-certainty
title: Emphasize distribution means in proportion to certainty
bibliography: references.bib
description: For small multivariate uncertainty views, use certainty-scaled mean emphasis
  on density plots to improve readability and address loss of individual sample locations
  for viewers inspecting manageable numbers of samples.
labels:
- purpose:refine
- basis:empirical
- lever:encoding
- operator:uncertainty
- density:sparse
- quality:readability
---

## Mean emphasis <!-- role: advice -->

Brighten or scale the center of each distribution on the density plot, and make the amount of emphasis rise with certainty. For example, multiply the distribution value at its mean so small-variance samples produce brighter centers than large-variance samples in scatter plots or parallel coordinates.

## Why mean emphasis works <!-- role: reason -->

Mean emphasis restores a discrete location cue without discarding the density summary. Because tighter normal distributions already peak higher at the mean, scaling the center strengthens certain values more than uncertain ones.

**Mechanism:** Viewers can see both where the distributions are centered and how broad they are. The centers of certain values remain easier to find, while uncertain values stay less prominent.

**Evidence:** The paper adds mean emphasis to density-based scatter plots and parallel coordinates, and explains that scaling the distribution mean creates a discrete feature that fades with uncertainty and helps viewers locate the contributing distributions when overplotting is still manageable [@fengMatchingVisualSaliency2010].

## When to use mean emphasis <!-- role: context -->

- **User Goal:** See where individual uncertain samples are centered without abandoning the density summary.
- **Task:** Locate contributing distributions while still reading overall density.
- **Data:** Multivariate uncertain data with distributions shown in a density plot.
- **Chart Setting:** Scatter plots or parallel coordinates with a small enough sample count that means do not heavily overlap.
- **Audience:** Analysts or domain experts inspecting individual sample locations.
- **Success Criterion:** The viewer can see both the width of each distribution and the location of its mean.

## When mean emphasis fails <!-- role: exceptions -->

**Break it when:** Many emphasized means overlap heavily or the plot is large enough that the added centers merge into clutter. **Why:** The density plot alone is the better summary once the emphasized centers stop being individually resolvable.

## Tradeoffs of mean emphasis <!-- role: costs -->

**Sacrifice:** You give up some of the clean continuous look of the plain density summary.
**Risk:** Too many emphasized centers can reintroduce clutter.
**Mitigation:** Reduce or remove mean emphasis when overlap becomes dominant and rely on the density image for summary.

## Common mistake with mean emphasis <!-- role: mistakes -->

**Mistake:** Overlay mean markers with equal prominence regardless of uncertainty. **Why it fails:** Saliency no longer matches confidence, so uncertain means can attract as much attention as certain ones.

## How to check mean emphasis <!-- role: check -->

**Failure Sign:** Broad uncertain means look as bright as tight certain means, or emphasized centers merge into a noisy layer.
**Quick Check:** Inspect whether the brightest emphasized centers belong to the smallest-variance distributions.
**Stronger Test:** Toggle mean emphasis on and off and confirm that it improves mean location lookup without obscuring the underlying density summary.

## How to fix mean emphasis <!-- role: fix -->

- Scale the center emphasis by certainty so tighter distributions receive stronger emphasis.
- Remove or weaken mean emphasis when many centers overlap.
- Keep the underlying density layer visible so viewers still see distribution width.
- Use the plain density plot alone when the chart's job is summary rather than individual mean lookup.
