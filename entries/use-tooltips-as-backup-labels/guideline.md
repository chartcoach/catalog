---
id: use-tooltips-as-backup-labels
title: Use tooltips only as backup labels for secondary categories
bibliography: references.bib
description: For interactive multi-category charts with limited label space, use tooltips
  on secondary categories to improve readability and address label crowding for readers
  exploring the chart while keeping important categories directly labeled.
labels:
- purpose:refine
- basis:heuristic
- lever:interaction-access
- component:tooltip:use
- component:label:use
- group-cardinality:many
- quality:readability:use
---

## Keep key labels on the chart <!-- role: advice -->

Use tooltips as a fallback for secondary categories, not as the main labeling system. For example, directly label the important lines or segments on the chart and let hover reveal the names of the remaining categories one at a time.

## Preserve scanning for the important categories <!-- role: reason -->

Tooltips save space, but they reveal only one label at a time. That makes them slower for scanning, searching, and comparing than direct labels, so they work best as support for the categories that could not be labeled directly.

**Mechanism:** Direct labels keep important identities visible at a glance, while tooltips handle the overflow without crowding the chart.

**Evidence:** The post says tooltips can reveal category labels on hover and are useful when there is not enough room for direct labels, but it also states that direct labels are more useful and that the most important categories should always be labeled directly rather than left to tooltips [@muth_fewer_colors_2022].

## Use when interaction can carry the overflow labels <!-- role: context -->

- **User Goal:** Show many categories without overcrowding the chart with labels.
- **Task:** Keep key categories readable while preserving access to secondary categories.
- **Data:** Many categories are present.
- **Chart Setting:** The chart is interactive and there is not enough space for all direct labels.
- **Audience:** Readers who can hover to inspect secondary categories.
- **Success Criterion:** Important categories are visible immediately and the remaining categories are still discoverable.

## Do not use for the most important categories <!-- role: exceptions -->

**Break it when:** A category is one of the most important ones in the chart. **Why:** Important categories should be labeled directly, not only on hover.

## Accept slower lookup for secondary categories <!-- role: costs -->

**Sacrifice:** Readers must hover to identify some categories.
**Risk:** Searching for a specific secondary category or comparing several secondary categories becomes slow because only one tooltip is visible at a time.
**Mitigation:** Keep direct labels for the important categories and use tooltips only for the remainder.

## Avoid making hover the only path to the main message <!-- role: mistakes -->

**Mistake:** Requiring readers to hover to identify the key categories. **Why it fails:** Readers cannot see the main categories immediately and cannot scan them quickly.

## Review the chart without hovering <!-- role: check -->

**Failure Sign:** The chart does not reveal its key categories until the viewer interacts with it.
**Quick Check:** Look at the chart with no hover state and confirm that the important categories are already labeled.
**Stronger Test:** Try finding and comparing two secondary categories; if that is slow, keep tooltips as a supplement rather than the main labeling system.

## Move only the overflow into tooltips <!-- role: fix -->

- Add direct labels to the most important categories on the chart itself.
- Keep tooltips for the remaining secondary categories.
- Replace some tooltip-only labels with direct labels if additional space becomes available.
