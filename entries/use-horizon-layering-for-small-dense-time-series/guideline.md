---
id: use-horizon-layering-for-small-dense-time-series
title: Use horizon layering when many time series must fit into very small charts
bibliography: references.bib
description: For compare tasks on dense ordered-time displays, prefer horizon graph
  layering on small time-series charts to improve readability and mitigate resolution
  loss from shrinking standard area plots for readers scanning many trends at once.
labels:
- purpose:refine
- basis:empirical
- task:compare
- time:ordered-time
- data:temporal
- quality:readability
- lever:layout-structure
- density:dense
---

## Horizon layering <!-- role: advice -->

Convert a small area chart into a horizon graph when you need to compare many time series in limited space. For example, mirror negative values into the positive region, then divide the values into bands and layer those bands so the chart preserves resolution while using about a quarter of the space of a standard area plot.

## Why horizon graphs help at small sizes <!-- role: reason -->

Shrinking a standard area chart reduces how much variation remains visible. Horizon layering increases data density without throwing away the time resolution, so more series can stay legible in the same space.

**Mechanism:** Mirroring and band layering compress vertical space while preserving the underlying temporal detail needed for comparison.

**Evidence:** The paper explains that mirroring negative values doubles the density of a standard area chart, and layering value bands doubles density again, producing a horizon graph that preserves data resolution in roughly one quarter of the space; it further states that horizon graphs have been found more effective than standard plots when chart sizes get quite small [@heerTourVisualizationZoo2010].

**Notes:** The paper also notes that horizon graphs take some time to learn.

## Where this applies <!-- role: context -->

- **User Goal:** Compare many time series at once.
- **Task:** Scan trends across multiple small time-series views.
- **Data:** Multiple ordered-time series, potentially with positive and negative values.
- **Chart Setting:** Space is tight and each series must be shown in a very small panel.
- **Audience:** Readers can spend some effort learning a compact time-series encoding.
- **Success Criterion:** More series fit on screen without losing the ability to see temporal variation.

## When not to use it <!-- role: exceptions -->

**Break it when:** The audience needs an immediately familiar time-series form or cannot spend time learning the encoding. **Why:** The paper states that horizon graphs take some time to learn.

## Tradeoffs of horizon layering <!-- role: costs -->

**Sacrifice:** You give up the immediate familiarity of a standard area chart.\
**Risk:** First-time readers may not understand the mirrored and layered bands.\
**Mitigation:** Use horizon layering where the space savings are necessary and chart size is already very small.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Simply shrinking standard area charts when many series must fit in one view. **Why it fails:** The reduced chart height makes the temporal variation harder to read, while horizon layering was designed to preserve resolution under tight space.

## How to check the chart <!-- role: check -->

**Failure Sign:** Tiny area charts become hard to compare once reduced to their final display size.\
**Quick Check:** View the chart at its actual small size and see whether peaks, dips, and sign changes are still distinguishable.\
**Stronger Test:** Compare the small standard area chart against a horizon version at the same size and check which one supports faster scanning across series.

## How to fix it <!-- role: fix -->

- Mirror negative values into the same vertical region as positive values.
- Split the value range into bands and layer those bands to compress height.
- Apply the horizon transformation only after confirming that the standard small area chart is too space-hungry at the target size.
