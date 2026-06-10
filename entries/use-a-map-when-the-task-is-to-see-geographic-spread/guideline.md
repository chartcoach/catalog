---
id: use-a-map-when-the-task-is-to-see-geographic-spread
title: Use a map when the task is to see geographic spread
bibliography: references.bib
description: For distribution tasks on geospatial data, use a map instead of a bar
  chart to improve insight and mitigate loss of spatial relationships for users exploring
  geographic spread.
labels:
- purpose:select
- basis:empirical
- task:distribute
- chart:map:use
- chart:bar:avoid
- data:geospatial
- quality:insight:use
- lever:chart-family
---

## Choose the spatial chart family <!-- role: advice -->

Choose a map when the job is to show where events or cases are distributed across space, and do not collapse that task into a bar chart. For example, use a map-like layout to show spread across islands or regions, and keep a bar chart only when the task is a simple count comparison by place rather than spatial spread.

## Preserve spatial relationships for spatial reasoning <!-- role: reason -->

A map keeps location, adjacency, and distribution visible in the display itself. A bar chart removes that spatial frame, so viewers must reason about spread without seeing where places are relative to each other.

**Mechanism:** Spatial arrangement supports direct reading of geographic patterns, while categorical bar positions hide the structure needed for spread analysis.

**Evidence:** The paper states that using a bar chart to represent the geographical spread of disease is less effective than using a map, and it also notes that the bar-chart alternative may still be better for a simple comparison task rather than a spatial one [@olaSimpleChartsDesign2016].

## Use when the task is spatial distribution <!-- role: context -->

- **User Goal:** See how a condition or event is distributed across places.
- **Task:** Explore spread, clustering, or geographic pattern.
- **Data:** Values are tied to identifiable locations or regions.
- **Chart Setting:** The visualization is meant to support analysis rather than only a simple categorical comparison.
- **Success Criterion:** Viewers can read spatial pattern directly from the display.

## Do not use when the task is only count comparison by place <!-- role: exceptions -->

**Break it when:** The primary task is a simple comparison of counts across named places rather than understanding geographic spread. **Why:** The paper explicitly notes that a bar-chart view may be better suited to that simpler comparison task.

## Trade off spatial insight against count-only simplicity <!-- role: costs -->

**Sacrifice:** You give up the very direct count-only comparison of a simple bar chart.
**Risk:** A map adds spatial structure that may be unnecessary when geography is not part of the question.
**Mitigation:** Keep the map for spread analysis, and use a separate simple count view only if the comparison task is also important.

## Avoid category-only placement for spatial tasks <!-- role: mistakes -->

**Mistake:** Using a bar chart to show geographic spread. **Why it fails:** The viewer sees counts by place name but not the spatial relationships that define spread.

## Test whether spatial pattern survives the chart choice <!-- role: check -->

**Failure Sign:** The viewer can compare place totals but cannot directly tell which places are near each other or how the pattern spreads across space.
**Quick Check:** Compare a bar-chart version and a map version of the same data and ask which one lets a reviewer see spatial pattern without extra recall.
**Stronger Test:** Ask a reviewer to describe the spread pattern directly from the chart; if they must reconstruct geography from labels alone, the bar chart is the wrong choice.

## Replace categorical placement with spatial placement <!-- role: fix -->

- Replace the categorical bar layout with a map-based spatial layout.
- Put the values on or within their geographic locations rather than on a categorical axis.
- Keep a separate bar chart only if you also need a simple by-place count comparison.
