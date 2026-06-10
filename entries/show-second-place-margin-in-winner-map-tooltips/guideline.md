---
id: show-second-place-margin-in-winner-map-tooltips
title: Show the second-place margin in tooltips on winner maps
bibliography: references.bib
description: For interactive inspection of winner-take-all district maps, use tooltip
  text on choropleth maps to improve insight and address winner-only summaries for
  readers checking how close the top two candidates were.
labels:
- purpose:refine
- basis:heuristic
- chart:choropleth
- data:geospatial
- component:tooltip:use
- operator:difference
- quality:insight:use
- lever:interaction-access
---

## Add the runner-up margin to the tooltip <!-- role: advice -->

Put the second-place margin into the tooltip on winner-take-all district maps. For example, on a map of district winners, add the vote difference between the winner and the runner-up to the hover text so close races can be found.

## Why the runner-up margin works <!-- role: reason -->

A winner-colored map hides how narrow the victory was, but the tooltip can reveal whether the first and second candidates were far apart or nearly tied.

**Mechanism:** Adding the gap between first and second place turns a winner-only map into a map that also supports inspection of close contests.

**Evidence:** The post says that one of the more interesting aspects of a first-vote winner map is the margin for the second-place candidate and describes adding that information to the tooltip because winner and runner-up shares are fairly close in some districts [@muth_german_election_2021].

## Use when the map shows district winners <!-- role: context -->

- **User Goal:** Let readers inspect how close district-level wins were.
- **Task:** Compare the winner with the runner-up within a district.
- **Data:** Winner-take-all district results with identifiable first and second place.
- **Chart Setting:** An interactive map with hover tooltips.
- **Success Criterion:** Readers can discover narrow wins without changing the main winner map.

## Do not use when the map is not a winner view <!-- role: exceptions -->

**Break it when:** The map is not showing winner-take-all district winners. **Why:** The post introduces the second-place margin specifically as extra detail for a first-vote winners map.

## Tradeoffs of the tooltip detail <!-- role: costs -->

**Sacrifice:** The second-place margin is hidden until interaction.
**Risk:** A reader can miss close races without hovering over districts.
**Mitigation:** Keep the winner visible in the main map and reserve the margin for the tooltip detail.

## Common failure around the tooltip detail <!-- role: mistakes -->

**Mistake:** Show only the winning party in the tooltip. **Why it fails:** The map still hides whether the race was close.

## Check whether closeness is visible <!-- role: check -->

**Failure Sign:** Hovering a district shows the winner but not the gap to second place.
**Quick Check:** Hover a close district; if you cannot tell how narrow the win was, the tooltip is missing the key comparison.
**Stronger Test:** Verify that the hover detail includes information for both first and second place or their margin.

## Fix the winner-only tooltip <!-- role: fix -->

- Add the vote difference between first and second place to the tooltip.
- Include runner-up information alongside the winner in the hover detail.
- Keep the main map focused on winners and move the closeness detail into the tooltip.
