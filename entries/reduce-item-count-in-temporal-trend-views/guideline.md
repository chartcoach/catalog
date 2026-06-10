---
id: reduce-item-count-in-temporal-trend-views
title: Reduce the number of displayed items in temporal trend views
bibliography: references.bib
description: For trend reading over ordered time, avoid dense item counts on multidimensional
  trend views to improve fidelity and mitigate clutter-driven misses for viewers.
labels:
- purpose:refine
- basis:empirical
- task:trend
- time:ordered-time
- density:dense
- temporal-pattern:dynamic
- quality:fidelity:use
- lever:layout-structure
---

## Reduce the number of visible item traces <!-- role: advice -->

Reduce the number of displayed items when many temporal traces share one view. For example, avoid filling an animation or trace overlay with so many items that paths blur together, and avoid a small-multiples grid so large that each trace becomes hard to read.

## Fewer items reduce clutter and tracking loss <!-- role: reason -->

Higher item counts make all three approaches harder to read, but in different ways. Dense animations and trace overlays create clutter and tracking loss, while dense small-multiples grids shrink each trace until it is hard to inspect.

**Mechanism:** Fewer displayed items reduce overlap in shared views and keep separate panels large enough to show each path clearly.

**Evidence:** Participants were significantly more accurate with the small dataset than with the large dataset, and the paper also reports that viewers often lost track of moving points and that higher item counts create clutter in animation and traces while shrinking small-multiple panels [@robertsonEffectivenessAnimationTrend2008].

**Notes:** The paper describes all three techniques as failing to scale much beyond about 200 displayed items.

## Use when many item-level paths compete for attention <!-- role: context -->

- **User Goal:** Find anomalies or compare item-level trends.
- **Task:** Read or present many temporal traces accurately.
- **Data:** Many items changing over time in a shared trend view or a grid of trend panels.
- **Chart Setting:** Animation, trace overlays, or small multiples are being used to show item-level temporal paths.
- **Audience:** Analysts or presentation viewers.
- **Success Criterion:** Better accuracy and less crowding.

## Do not use dense reduction tactics when item-level anomalies must remain visible <!-- role: exceptions -->

**Break it when:** The only way to reduce crowding is to aggregate items, and the task depends on seeing item-level anomalies. **Why:** The paper notes that aggregation can reduce clutter and occlusion but may hide anomalies of interest.

## Tradeoffs of reducing item count <!-- role: costs -->

**Sacrifice:** You may give up full item coverage in one view.
**Risk:** If you collapse items together, important anomalies can disappear.
**Mitigation:** Keep item-level views for anomaly detection and avoid aggregation when the anomaly itself is the target.

## Common failure around dense trend views <!-- role: mistakes -->

**Mistake:** Solving crowding only by aggregating items into larger groups. **Why it fails:** The reduced view may hide the very anomalies the reader needs to detect.

## How to test item density <!-- role: check -->

**Failure Sign:** Paths blur together in shared views, panels become tiny, or viewers report losing track of moving points.
**Quick Check:** Compare one representative task with the full item set and with a reduced item set; if the dense view causes misses or tracking complaints, keep the reduced view.
**Stronger Test:** Verify that each remaining path can be individually tracked without replay or squinting.

## What to change <!-- role: fix -->

- Show a smaller set of items in the temporal view.
- Do not rely on aggregation when the task is to spot item-level anomalies.
- Keep a small-multiples grid only while each panel remains large enough to show its trace clearly.
- If a shared view is still crowded after reduction, move the analysis to a small-multiples layout.
