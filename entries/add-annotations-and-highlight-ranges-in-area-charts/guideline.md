---
id: add-annotations-and-highlight-ranges-in-area-charts
title: Add annotations and highlight ranges to explain area charts
bibliography: references.bib
description: For explaining change over ordered time, use text annotation on area
  charts to improve insight and mitigate unexplained patterns for readers trying to
  understand what is happening.
labels:
- purpose:refine
- basis:heuristic
- time:ordered-time
- chart:area
- quality:insight:use
- lever:text-annotation
- component:annotation:use
- polish:annotation
---

## Annotate the important change <!-- role: advice -->

Add annotations and highlight ranges to explain the important patterns in an area chart. For example, place a note on the chart or shade a time span to explain why the areas change.

## Why explanations help on area charts <!-- role: reason -->

Area charts leave enough room for explanatory notes inside or around the plotting area. These additions help readers connect visible changes to the explanation.

**Mechanism:** Annotations and highlighted ranges tell readers what part of the chart deserves attention and help them figure out what is going on.

**Evidence:** The source recommends using annotations and highlight ranges to add explanations to area charts, noting that they have enough space for these additions and that the additions help readers understand the chart [@muth_area_charts_2018].

## Use when the chart needs explanation <!-- role: context -->

- **User Goal:** Explain why the chart changes or what a period means.
- **Task:** Guide readers to the important event, pattern, or range.
- **Data:** Temporal values shown in an area chart.
- **Chart Setting:** The chart has enough open space to place notes or highlighted ranges.
- **Audience:** Readers who need help understanding what is going on.
- **Success Criterion:** Readers can connect the visual change to the explanation on the chart.

## Do not use when there is nothing to explain <!-- role: exceptions -->

**Break it when:** The chart has no event, change, or period that needs explanation. **Why:** The source recommends annotations to add explanations, not as decoration.

## What you give up <!-- role: costs -->

**Sacrifice:** You use some of the available chart space for explanatory text or highlighted ranges.
**Risk:** Notes that do not explain a real change add little value.
**Mitigation:** Reserve annotations for the part of the chart that needs explanation.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Leaving important changes unexplained even though the chart has room for notes. **Why it fails:** Readers must guess why the pattern changes instead of seeing the explanation where the change happens.

## How to test the revision <!-- role: check -->

**Failure Sign:** Readers can see a change in the chart but cannot tell what explains it.
**Quick Check:** Ask whether the important change or time span is explicitly marked on the chart.
**Stronger Test:** Add a note or highlighted range and check whether the chart now tells readers what is going on without extra explanation elsewhere.

## What to change <!-- role: fix -->

- Add a short annotation at the key change.
- Highlight the relevant time range directly on the chart.
- Remove notes that do not explain a visible pattern or period.
