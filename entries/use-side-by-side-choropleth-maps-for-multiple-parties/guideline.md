---
id: use-side-by-side-choropleth-maps-for-multiple-parties
title: Place choropleth maps side by side when comparing multiple parties
bibliography: references.bib
description: For comparing multiple groups across the same districts, use a small-multiple
  layout instead of a single choropleth map to improve insight and mitigate one-map
  overload for readers scanning regional patterns.
labels:
- purpose:select
- basis:heuristic
- task:compare
- structure:small-multiples:use
- structure:single-view:avoid
- chart:choropleth
- data:geospatial
- quality:insight:use
- lever:layout-structure
---

## Split the map into side-by-side panels <!-- role: advice -->

Place multiple choropleth maps side by side when you need to show vote shares for more than one party. For example, use a few aligned district maps for several parties instead of forcing one choropleth map to carry all parties’ vote shares at once.

## Why side-by-side panels work <!-- role: reason -->

Separate panels let each district keep one value per map, while the shared geography across panels makes cross-party patterns visible.

**Mechanism:** One district can only encode one party’s vote share in one choropleth at a time, so splitting the view prevents that encoding conflict.

**Evidence:** The post states that each district in a choropleth map can only show the vote share of one party at a time and recommends placing a few maps next to each other to show multiple parties and reveal patterns [@muth_german_election_2021].

## Use when one map is not enough <!-- role: context -->

- **User Goal:** Compare regional patterns for several parties.
- **Task:** Scan the same districts across multiple vote-share views.
- **Data:** Multiple district-level vote-share series for the same geography.
- **Chart Setting:** The maps can be placed next to each other.
- **Success Criterion:** Readers can compare patterns across parties without losing the district geography.

## Do not use when only one party is being shown <!-- role: exceptions -->

**Break it when:** The map needs to show the vote share of only one party. **Why:** The post says a single choropleth can show one party’s vote share at a time.

## Tradeoffs of side-by-side panels <!-- role: costs -->

**Sacrifice:** The layout uses several maps instead of one.
**Risk:** The comparison weakens if the maps are not placed next to each other.
**Mitigation:** Keep the maps adjacent so readers can scan across them.

## Common failure around side-by-side panels <!-- role: mistakes -->

**Mistake:** Try to show several parties’ vote shares in one choropleth map. **Why it fails:** Each district can only show one party’s value at a time.

## Check whether one map is overloaded <!-- role: check -->

**Failure Sign:** One choropleth is expected to represent more than one party’s district vote share.
**Quick Check:** Count how many party values each district must show; if it is more than one, compare the single-map attempt with a side-by-side layout.
**Stronger Test:** Verify that each panel reuses the same district geography so the regional patterns can be compared across panels.

## Fix the overloaded choropleth <!-- role: fix -->

- Split the single map into separate choropleth panels.
- Place the panels next to each other.
- Keep the same district geography across all panels.
