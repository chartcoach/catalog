---
id: split-multiple-axis-charts-into-separate-charts
title: Split charts with multiple X or Y axes into separate charts
bibliography: references.bib
description: For multi-measure reading and comparison, prefer separate-chart layout
  structure on views that would otherwise use more than one X or Y axis to prevent
  cognitive overload and mitigate ambiguous axis interpretation for broad audiences.
labels:
- purpose:select
- basis:accessibility
- structure:multi-view:use
- structure:single-view:avoid
- measure:multi
- lever:layout-structure
- needs:cognitive
- quality:accessibility
---

## Split the measures into separate charts <!-- role: advice -->

Use separate charts instead of adding a second X or Y axis when one view would need multiple axes. For example, replace one combined multi-axis chart with two charts presented separately before any combined view.

## Why separate axes work <!-- role: reason -->

Multiple axes force readers to track more than one scale in the same view and make interpretation more attentive than immediate. Splitting the measures into separate charts keeps each scale unambiguous and lowers the working-memory burden.

**Mechanism:** Separate charts keep one axis system per view, so readers do not need to decode which scale applies to which marks.

**Evidence:** Chartability defines inappropriate information complexity to include charts with more than one X or Y axis and directs authors to present two charts separately first; the linked statistical graphics guideline likewise recommends avoiding dual axes to reduce cognitive limits in graph interpretation [@elavskyHowAccessibleMy2022; @ed_design_guidelines].

**Notes:** Claims that dual-axis charts work for trained experts are treated cautiously because audience skill is hard to verify and the accessibility benefit is unclear.

## Use when a second axis is being considered <!-- role: context -->

- **User Goal:** Show more than one measured variable without overloading the reader.
- **Data:** Multiple measures that tempt adding another X or Y axis.
- **Chart Setting:** A single chart currently has, or is planned to have, more than one X or Y axis.
- **Audience:** Broad or mixed-skill readers, or any audience whose chart-reading skill is not known.
- **Success Criterion:** Readers can interpret each measure without ambiguous scale matching or extra attentive effort.

## Do not apply when there is no extra axis <!-- role: exceptions -->

**Break it when:** The chart uses only one X axis and one Y axis. **Why:** This rule addresses the added complexity created by multiple axes in one chart.

## Tradeoffs of splitting the view <!-- role: costs -->

**Sacrifice:** You give up a single compact combined chart.
**Risk:** Splitting views when no extra axis is needed adds unnecessary structure.
**Mitigation:** Apply the split only when a second X or Y axis would otherwise be introduced.

## Common multiple-axis mistake <!-- role: mistakes -->

**Mistake:** Keep multiple measures in one chart by adding a second X or Y axis because some readers may be experts. **Why it fails:** Reader skill is hard to verify, and the source treats multi-axis charts as inaccessible to a broad audience and likely even expert readers.

## Check for multiple-axis complexity <!-- role: check -->

**Failure Sign:** One chart contains more than one X or more than one Y axis.
**Quick Check:** Compare the current chart to a version split into two charts; if the current version needs a second axis to fit both measures, choose the split version.
**Stronger Test:** Verify that each resulting chart can show its measure with only one X axis and one Y axis before presenting any combined view.

## Fix the extra axis <!-- role: fix -->

- Remove the extra X or Y axis from the combined chart.
- Put each measure in its own chart instead of keeping both measures on one multi-axis view.
- Present the two charts separately before any combined version.
