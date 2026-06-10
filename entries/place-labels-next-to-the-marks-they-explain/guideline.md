---
id: place-labels-next-to-the-marks-they-explain
title: Place labels next to the marks they explain
bibliography: references.bib
description: For quick lookup on color-coded charts, prefer nearby labels over separated
  legends to improve readability and mitigate repeated eye-travel for readers scanning
  the graphic.
labels:
- purpose:refine
- basis:heuristic
- quality:readability
- lever:text-annotation
- component:label:use
- component:legend:avoid
---

## Directly label the marks <!-- role: advice -->

Place labels or explanations beside the marks they describe instead of sending readers to a distant legend. For example, label line series on the lines themselves or move bar explanations next to the colored bars instead of keeping a color key in a corner.

## Why nearby labels work <!-- role: reason -->

Readers waste time when they have to shuttle their eyes between a mark and a far-away key. Nearby labels keep decoding local, so identification becomes faster and less frustrating.

**Mechanism:** Bringing the explanation to the mark removes repeated back-and-forth lookups, which reduces search effort and makes the chart easier to scan.

**Evidence:** The post explicitly warns against charts with a color key in one corner and the colored lines or bars elsewhere, and recommends bringing elements and their explanations as close together as possible, including labeling lines directly rather than relying on a separate legend [@muth_readers_time_2017].

## Use when the chart requires mark-to-label lookup <!-- role: context -->

- **User Goal:** Identify what a colored line, bar, or other mark represents quickly.
- **Task:** Lookup rather than prolonged exploration.
- **Chart Setting:** The chart uses colored marks and would otherwise rely on a separate color key or legend.
- **Audience:** Readers scanning the chart and asking what a given color represents.
- **Success Criterion:** Readers can identify each highlighted element without looking to another corner of the chart.

## Do not use when small-screen space removes the labels <!-- role: exceptions -->

**Break it when:** The chart must collapse to a very small mobile view and on-mark labels cannot survive the reduced space. **Why:** The source notes that rich annotations often disappear in mobile-first versions of the same chart.

## Tradeoffs of direct labels <!-- role: costs -->

**Sacrifice:** Some layout flexibility and responsiveness.\
**Risk:** Direct labels can disappear or become hard to preserve in very small views.\
**Mitigation:** If small screens force fewer labels, use animation to communicate some of the same information.

## Common failure mode: separating the legend from the marks <!-- role: mistakes -->

**Mistake:** Keeping a distant legend or color key while the marks sit elsewhere in the chart. **Why it fails:** Readers have to look back and forth repeatedly to decode the display.

## Check whether label lookup stays local <!-- role: check -->

**Failure Sign:** To decode a mark, you look from the mark to a far-away key and back again.\
**Quick Check:** Pick any colored element and see whether its explanation is visible in the same local area.\
**Stronger Test:** Shrink the chart to a smaller view and see whether the nearby labels still survive; if they vanish, the chart needs a small-screen fallback.

## Fix the chart by moving labels onto the marks <!-- role: fix -->

- Remove the separated legend when the marks can be labeled directly.
- Put the series name or explanation on the line, bar, or immediately beside it.
- Rework the layout so the explanation sits near the mark instead of in a distant corner.
- If small screens cannot hold the direct labels, replace some of the lost explanation with animation.
