---
id: add-tooltips-for-region-names-and-values
title: Add tooltips for region names and values
bibliography: references.bib
description: For interactive choropleths, use tooltips on regions to improve readability
  and mitigate hidden names and values for readers inspecting specific places.
labels:
- purpose:refine
- basis:heuristic
- chart:choropleth
- component:tooltip:use
- quality:readability
- lever:interaction-access
- reading-mode:lookup
---

## Tooltip content <!-- role: advice -->

Add tooltips that reveal each region's name and underlying value. For example, use the tooltip to show the region label, the mapped number, and brief extra information that reminds readers what they are seeing.

## Why hover detail helps maps <!-- role: reason -->

Region names and values are hard to read directly from a filled map.

**Mechanism:** Tooltips let readers inspect one place at a time and recover the exact value and region name without cluttering the map. They can also restate the map's subject and add a small amount of extra regional context.

**Evidence:** The post says tooltips are a great option for communicating each region's name and value because those are otherwise hard to read, and that tooltips can also add extra information and remind readers what they are seeing [@muth_choroplethmaps_2018].

## Use when the map supports interactive lookup <!-- role: context -->

- **User Goal:** Inspect a specific region.
- **Task:** Look up the name and exact value for one mapped area.
- **Data:** Regional values shown by color.
- **Chart Setting:** The choropleth supports tooltips.
- **Audience:** Readers moving from overview to lookup.
- **Success Criterion:** A reader can identify a region and retrieve its exact value on demand.

## Do not rely on tooltips alone when geography is unfamiliar <!-- role: exceptions -->

**Break it when:** Readers are unlikely to know the mapped area well. **Why:** The post says labels become more important as reader knowledge of the area decreases.

## Costs of tooltip-based lookup <!-- role: costs -->

**Sacrifice:** Names and exact values are not visible all at once.
**Risk:** Readers must inspect regions one by one to retrieve detail.
**Mitigation:** Pair tooltips with labels when readers also need help locating places.

## Common hidden-detail failure <!-- role: mistakes -->

**Mistake:** Rely on color alone to communicate region names and exact values. **Why it fails:** Readers cannot easily recover the specific place and number from the map itself.

## Check whether the tooltip carries the needed detail <!-- role: check -->

**Failure Sign:** A reader cannot identify a region's name or exact value without searching elsewhere.
**Quick Check:** Hover or tap a region and verify that the tooltip shows its name and underlying value.
**Stronger Test:** Confirm that the tooltip also briefly restates what the map is showing when that context would otherwise be easy to forget.

## Edit the tooltip <!-- role: fix -->

- Add the region name to the tooltip.
- Add the exact mapped value to the tooltip.
- Add a short reminder of what the map measures.
- Add brief extra regional information only if it helps interpretation.
