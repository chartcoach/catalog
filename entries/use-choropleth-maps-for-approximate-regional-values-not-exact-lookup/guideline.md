---
id: use-choropleth-maps-for-approximate-regional-values-not-exact-lookup
title: Use choropleth maps for approximate regional values, not exact lookup
bibliography: references.bib
description: For regional lookup and comparison, use approximate-value interpretation
  on choropleth maps to improve fidelity and mitigate mistaken exact-value lookup
  for novice readers.
labels:
- purpose:refine
- basis:empirical
- chart:choropleth
- data:geospatial
- lever:encoding
- operator:lookup
- quality:fidelity
- literacy:novice
---

## Treat color fills as ranges <!-- role: advice -->

Treat choropleth map colors as approximate ranges, not exact numbers. For example, use the map to compare regions or find the highest-valued region, but avoid asking the reader to read a precise regional value from the fill color alone.

## Why approximate reading fits the map <!-- role: reason -->

A choropleth uses color bins to segment regions into ranges. That supports approximate lookup and comparison, but not precise numerical reading.

**Mechanism:** The fill color tells the reader which range a region belongs to. Multiple exact values can map to the same color, so exact lookup is not visually recoverable from the map alone.

**Evidence:** In the VLAT blueprint, choropleth maps were marked as supporting only approximate-value tasks because the visual objects represent approximately segmented ranges rather than exact regional values [@leeVLATDevelopmentVisualization2017].

## Use when regional comparison is enough <!-- role: context -->

- **User Goal:** Compare regions or read an approximate regional level.
- **Task:** Approximate lookup, extremum finding, or regional comparison.
- **Data:** Geospatial regions colored by a quantitative measure.
- **Chart Setting:** A choropleth map with segmented legend ranges.
- **Audience:** Novice or non-expert readers.
- **Success Criterion:** Readers can identify relative ordering or approximate level by region.

## Do not use when the reader needs exact per-region numbers <!-- role: exceptions -->

**Break it when:** The task requires a precise numeric value for each region. **Why:** The color fills show binned ranges, not exact regional values.

## Tradeoffs of using approximate map reading <!-- role: costs -->

**Sacrifice:** You give up precise regional value lookup from the fill color alone.\
**Risk:** Readers may over-read small color differences as exact numeric differences.\
**Mitigation:** Keep the intended reading at the level of approximate value, ranking, or comparison.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Writing the task as an exact numeric lookup from the choropleth color. **Why it fails:** The color encodes a range, so the map cannot justify a precise single value.

## How to test the map <!-- role: check -->

**Failure Sign:** The desired answer is a precise number even though the region is encoded only by a color bin.\
**Quick Check:** Ask whether the reader can answer only with a range or approximation from the legend.\
**Stronger Test:** If several exact values would map to the same fill color, the choropleth cannot support exact lookup.

## What to change <!-- role: fix -->

- Rewrite the task or annotation to ask for an approximate value, rank, or regional comparison.
- Remove precise numeric claims that rely only on the fill color.
- Replace the choropleth when exact regional lookup is the main requirement.
