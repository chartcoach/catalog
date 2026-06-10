---
id: use-choropleths-for-region-level-values
title: Use a choropleth for values attached to administrative regions
bibliography: references.bib
description: For showing geospatial values by administrative region, prefer a choropleth
  over a symbol map to improve fidelity and mitigate treating region data as exact
  locations for map readers.
labels:
- purpose:select
- basis:heuristic
- chart:choropleth:use
- chart:map:avoid
- data:geospatial
- lever:chart-family
- quality:fidelity
---

## Region fills for region data <!-- role: advice -->

Fill administrative regions when the data is reported for regions rather than for exact locations. For example, map turnout or crime rates by municipality or province with a choropleth instead of placing symbols as if each value belonged to a single point.

## Why filled regions match region-level data <!-- role: reason -->

Region-level data belongs to boundaries, not to isolated points. A choropleth keeps the geographic unit of the data visible.

**Mechanism:** Coloring whole regions matches how the values are stored and read, so the map does not imply false point precision.

**Evidence:** Choropleth maps are recommended for data available in administrative regions such as municipalities or provinces, while symbol maps are reserved for lots of specific locations [@muth_chart_types_guide_2025].

## Use when each value belongs to a named region <!-- role: context -->

- **User Goal:** Show a geographic pattern across administrative areas.
- **Task:** Compare region-level values on a map.
- **Data:** Geospatial values attached to municipalities, provinces, or similar regions.
- **Chart Setting:** A map where the data is aggregated by boundary.
- **Audience:** Map readers looking for regional patterns.
- **Success Criterion:** The map makes the relevant regions and their values immediately visible.

## Do not use when the data is a set of exact places <!-- role: exceptions -->

**Break it when:** The dataset consists of many specific locations rather than region-level aggregates. **Why:** Symbol maps are the right choice for mapping lots of exact places.

## Costs of switching to a choropleth <!-- role: costs -->

**Sacrifice:** You give up point-by-point location markers.\
**Risk:** If the data is actually point-based, a choropleth implies an aggregation the data does not have.\
**Mitigation:** Use choropleths only for values that belong to administrative regions.

## Common failure with regional map data <!-- role: mistakes -->

**Mistake:** Use point symbols for values that are only available by municipality, province, or another administrative region. **Why it fails:** The map stops matching the geographic unit of the data.

## Check whether the geographic unit is a region rather than a point <!-- role: check -->

**Failure Sign:** Each data row is an administrative area, not an exact place.\
**Quick Check:** Compare a choropleth draft with a symbol-map draft; if the symbol map only stands in for whole regions, keep the choropleth.\
**Stronger Test:** Ask whether the data can be joined to boundaries directly without inventing exact point locations.

## Fix the region-level map <!-- role: fix -->

- Join the values to administrative boundaries.
- Encode the values by filling each region lighter or darker.
- Remove point symbols that imply an exact location the data does not provide.
