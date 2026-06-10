---
id: use-choropleth-maps-for-regional-vote-patterns
title: Use a choropleth map to show regional vote patterns
bibliography: references.bib
description: For regional comparison across districts, use a choropleth map instead
  of a bar chart on geospatial vote results to improve insight and mitigate non-spatial
  summaries for readers who need to see where support is concentrated.
labels:
- purpose:select
- basis:heuristic
- task:distribute
- chart:choropleth:use
- chart:bar:avoid
- data:geospatial
- quality:insight:use
- lever:chart-family
---

## Use the geographic view <!-- role: advice -->

Choose a choropleth map when the chart’s job is to show where vote shares or gains are distributed. For example, color each district by one party’s vote share or by the party with the biggest gain rather than using a bar or column chart that only shows totals.

## Why the geographic view works <!-- role: reason -->

A choropleth map preserves location, so readers can see regional concentration and spread instead of only national totals.

**Mechanism:** Coloring districts ties the values to place, which makes geographic patterns visible.

**Evidence:** The post recommends showing election results not only with normal bar or column charts of party shares but also with maps to show their regional distribution, including vote share by district and which party gained most in each district [@muth_german_election_2021].

## Use when place is part of the message <!-- role: context -->

- **User Goal:** Show where parties are strong or where gains happened.
- **Task:** Compare regions or districts.
- **Data:** District-level election results or district-level change values.
- **Chart Setting:** Geography is meaningful to the interpretation.
- **Success Criterion:** Readers can identify regional differences directly from the display.

## Do not use when only national totals matter <!-- role: exceptions -->

**Break it when:** The chart only needs to show overall party vote shares with no geographic question. **Why:** The post treats bar or column charts as the standard summary for that non-spatial task.

## Tradeoffs of the geographic view <!-- role: costs -->

**Sacrifice:** A map shifts attention from national totals to districts and regions.
**Risk:** If the reader only needs overall shares, the added geography is not the main message.
**Mitigation:** Use a bar or column chart when the task is only to compare aggregate party shares.

## Common failure around the geographic view <!-- role: mistakes -->

**Mistake:** Use a totals bar chart when the question is where parties succeeded or where gains changed by district. **Why it fails:** The bars remove the regional pattern that the map is meant to show.

## Check whether geography is necessary <!-- role: check -->

**Failure Sign:** The story asks where support is concentrated, but the chart contains no district geography.
**Quick Check:** Compare a district map with an aggregate bar chart; if only the map preserves the regional pattern, choose the map.
**Stronger Test:** Confirm that a reader can locate differences by district from the graphic alone.

## Fix the non-spatial summary <!-- role: fix -->

- Replace the aggregate bar view with a district choropleth map.
- Encode either one party’s vote share or the category with the biggest gain in each district.
- Keep the geographic units visible so the regional pattern can be read directly.
