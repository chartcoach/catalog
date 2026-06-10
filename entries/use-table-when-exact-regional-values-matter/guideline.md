---
id: use-table-when-exact-regional-values-matter
title: Use a table when exact regional values or tiny regions matter
bibliography: references.bib
description: For exact lookup and comparison of regional values, prefer a table over
  a choropleth on geospatial data to improve readability and mitigate color-based
  imprecision when subtle differences or very small regions matter.
labels:
- purpose:select
- basis:heuristic
- chart:table:use
- chart:choropleth:avoid
- data:geospatial
- quality:readability
- lever:chart-family
- reading-mode:exact
---

## Chart family for exact regional reading <!-- role: advice -->

Replace the choropleth with a table when readers need exact regional values or when the important regions are too small to read on the map. For example, list each region with its value instead of asking readers to judge subtle color differences or locate tiny polygons.

## Why exact reading breaks on choropleths <!-- role: reason -->

Choropleths are good at showing the big picture, not at supporting exact value reading from color or very small shapes.

**Mechanism:** Color differences are hard to read precisely, and small regions can disappear as readable units. A table makes the value and the region name directly accessible.

**Evidence:** The post says choropleth maps are great for the big picture but not for subtle differences, and recommends another chart type, a table, or text when exact differences matter or key regions are too small to show [@muth_choroplethmaps_2018].

## Use when precision matters more than pattern <!-- role: context -->

- **User Goal:** Look up exact regional values.
- **Task:** Compare close values or inspect specific small regions.
- **Data:** Regional values with subtle differences or important small-area units.
- **Chart Setting:** A choropleth draft makes values hard to distinguish by color.
- **Audience:** Readers who need exact reading rather than a broad spatial impression.
- **Success Criterion:** Readers can find the value for each important region directly.

## Do not use when the main goal is the big picture <!-- role: exceptions -->

**Break it when:** The main goal is to show broad regional pattern rather than exact values. **Why:** The post says choropleths are strong for seeing the big picture.

## Costs of moving from map to table <!-- role: costs -->

**Sacrifice:** You lose the immediate spatial overview.
**Risk:** Regional clustering becomes less visible without the map.
**Mitigation:** Keep the table for exact reading only when the precise numbers or tiny regions are the main need.

## Common precision failure <!-- role: mistakes -->

**Mistake:** Keep adding color steps to a choropleth to force exact reading. **Why it fails:** Readers still have to estimate values from color, and tiny regions remain hard to inspect.

## Decide between choropleth and table <!-- role: check -->

**Failure Sign:** Readers cannot confidently distinguish close values or find the key small regions on the map.
**Quick Check:** Compare a choropleth draft and a table draft for the same regions and see which one lets a reader identify an exact value faster.
**Stronger Test:** Test the two closest values and the smallest important region; if the map does not support both cleanly, use the table.

## Edit the display for exact regional lookup <!-- role: fix -->

- Replace the choropleth with a table of region names and values.
- Sort or scan the table so the important regions are easy to find.
- Remove claims that require precise reading from color differences.
- Keep the map only if the story truly depends on the spatial pattern.
