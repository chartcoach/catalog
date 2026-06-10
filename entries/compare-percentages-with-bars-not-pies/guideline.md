---
id: compare-percentages-with-bars-not-pies
title: Use bars instead of pie or donut slices for percentage comparisons
bibliography: references.bib
description: For comparing shares across categories, prefer bar charts over pie or
  donut charts to improve readability and mitigate hard-to-see percentage differences
  for general audiences.
labels:
- purpose:select
- basis:heuristic
- chart:bar:use
- chart:pie-donut:avoid
- operator:part-whole
- reading-mode:exact
- lever:chart-family
- quality:readability
---

## Bar encoding for shares <!-- role: advice -->

Replace circle sectors with bars when readers need to compare percentages across categories. For example, show election results as bars instead of a pie or donut when small gaps such as a 3 percentage-point difference should be easy to see.

## Why bars make percentage gaps easier to see <!-- role: reason -->

Aligned lengths are easier to compare than circle sections. Small differences that nearly disappear in a pie or donut become visible in bars.

**Mechanism:** Bars put percentages on a common baseline, making gaps and ranking easier to judge than with angles or arc lengths.

**Evidence:** Pie, donut, and parliament charts clearly signal that the values are percentages, but circle sections are described as not easy to compare, while a 3% difference is easy to spot in a bar chart and practically invisible in a pie or donut [@muth_chart_types_guide_2025].

## Use when percentage comparison is the main job <!-- role: context -->

- **User Goal:** Compare category shares or rank categories by percentage.
- **Task:** Detect small differences between percentages.
- **Data:** One percentage value per category.
- **Chart Setting:** A share chart where the reader needs comparison more than decoration.
- **Audience:** A mainstream audience.
- **Success Criterion:** Small percentage gaps are easy to spot.

## Do not use when the main need is only to signal that values are percentages <!-- role: exceptions -->

**Break it when:** Fine comparison is not important and the chart mainly needs to make clear that it is showing shares rather than absolute numbers. **Why:** Pie and donut charts state that percentages are being shown very obviously.

## Costs of replacing circle sectors <!-- role: costs -->

**Sacrifice:** You lose the immediate visual cue that the display is about percentages rather than absolute totals.\
**Risk:** If exact comparison is not the real task, the swap may not add much.\
**Mitigation:** Make the switch when the key message depends on comparing percentage differences.

## Common failure with share charts <!-- role: mistakes -->

**Mistake:** Keep a pie or donut chart when the reader must spot small differences between categories. **Why it fails:** Circle sections make close percentage comparisons hard to see.

## Check whether the share chart supports comparison <!-- role: check -->

**Failure Sign:** Small percentage differences are hard to judge in the pie or donut.\
**Quick Check:** Build both a bar version and a pie or donut version of the same percentages; if the bar version makes the key ranking or gap obvious, use bars.\
**Stronger Test:** Ask whether a reader can reliably tell which category is slightly larger without reading every number.

## Fix the share comparison <!-- role: fix -->

- Replace the pie or donut with a bar chart.
- Keep the same percentage values and compare them as aligned lengths.
- Reserve the pie or donut form for cases where exact percentage comparison is not the point.
