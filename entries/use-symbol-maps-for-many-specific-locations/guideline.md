---
id: use-symbol-maps-for-many-specific-locations
title: Use a symbol map for many specific locations
bibliography: references.bib
description: For showing many exact locations on a map, prefer a symbol map over a
  choropleth to improve fidelity and mitigate forcing point data into administrative
  regions for map readers.
labels:
- purpose:select
- basis:heuristic
- chart:map:use
- chart:choropleth:avoid
- data:geospatial
- density:dense
- lever:chart-family
- quality:fidelity
---

## Point symbols for exact locations <!-- role: advice -->

Plot exact locations with symbols when the data consists of many places. For example, show universities, venues, or other mapped sites as points instead of coloring surrounding regions.

## Why point symbols fit exact locations <!-- role: reason -->

Exact places should appear where they actually are. A choropleth substitutes regional shading for point data and changes the geographic meaning of the dataset.

**Mechanism:** Symbol maps preserve the location of each place instead of collapsing many places into region-level color fills.

**Evidence:** Symbol maps are recommended when there are lots of specific locations to map, whereas choropleths are introduced for values available in administrative regions [@muth_chart_types_guide_2025].

## Use when the dataset is a list of places <!-- role: context -->

- **User Goal:** Show where many places are located.
- **Task:** Map exact locations rather than regional aggregates.
- **Data:** Geospatial records with specific places to plot.
- **Chart Setting:** A map of many individual locations.
- **Audience:** Map readers looking for where places are.
- **Success Criterion:** The map shows the actual placement of the locations instead of a regional summary.

## Do not use when the values are only available by region <!-- role: exceptions -->

**Break it when:** The data is aggregated by municipalities, provinces, or other administrative regions. **Why:** Choropleths are suited to region-level values.

## Costs of switching to symbols <!-- role: costs -->

**Sacrifice:** You give up the broad region-by-region color shading of a choropleth.\
**Risk:** If the data is regional rather than point-based, symbols imply false precision.\
**Mitigation:** Use symbols only when the data really consists of specific locations.

## Common failure with point-based map data <!-- role: mistakes -->

**Mistake:** Force exact-location data into a choropleth. **Why it fails:** The map no longer shows where the places actually are.

## Check whether the data names exact places <!-- role: check -->

**Failure Sign:** The dataset lists many concrete locations to plot rather than only region names.\
**Quick Check:** Compare a symbol-map draft with a choropleth draft; if the choropleth requires inventing regional summaries, keep the symbol map.\
**Stronger Test:** Ask whether each record can be placed as a location without first aggregating it to a boundary.

## Fix the exact-location map <!-- role: fix -->

- Place each specific location as a symbol on the map.
- Remove regional fills that are not backed by region-level values.
- Keep choropleth shading only for data that is actually aggregated by administrative area.
