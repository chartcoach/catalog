---
id: balance-white-space-around-interval-marks
title: Balance white space around interval marks
bibliography: references.bib
description: For visual reading of interval charts, prefer balanced white space in
  mark spacing and chart padding on interval-based chart layouts to improve accessibility
  and mitigate thin marks, oversized gaps, and crowded structure for readers interpreting
  chart structure visually.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:layout-structure
- polish:spacing
- aesthetic:composition:use
---

## Balance white space around interval marks <!-- role: advice -->

Use balanced white space around interval marks and related chart elements so the structure is easy to see. For example, on a bar chart, avoid bars that become thin with large gaps between them, and avoid the reverse layout where bars or labels are packed too tightly.

## Why balanced spacing helps perception <!-- role: reason -->

White space acts as chart structure. Balanced spacing helps readers separate marks, groups, and labels without losing the overall pattern, while extreme spacing makes marks feel either isolated or crowded.

**Mechanism:** Balanced spacing improves visual grouping and readability. Extreme spacing breaks perceivability by making interval marks too thin and separated or too compressed to parse cleanly.

**Evidence:** Chartability identifies inappropriate spacing as an accessibility issue and specifically warns that too much or too little white space on charts with intervals, such as thin bars with large gaps or the reverse, can create perceivable and understandable problems [@elavskyHowAccessibleMy2022]. The linked design references describe whitespace as a critical design element for readability, balance, grouping, and guiding the viewer's eye [@towardsdatascience_data_visualisation; @calliaweb_whitespace_not].

**Notes:** This guideline is based on community practice, and the source notes a research gap around white space in accessible data visualization.

## When to apply spacing balance <!-- role: context -->

- **User Goal:** Identify chart structure and intervals quickly.
- **Data:** Repeated interval marks or grouped visual elements where gap size changes how the chart is perceived.
- **Chart Setting:** A visual chart that uses white space or padded spacing to separate marks, labels, or groups.
- **Audience:** Readers relying on visual parsing of the chart.
- **Success Criterion:** Marks, gaps, and groups are easy to identify without looking isolated or crowded.

## When this spacing rule does not apply <!-- role: exceptions -->

**Break it when:** The chart does not contain interval marks or grouped visual elements whose spacing can be adjusted. **Why:** This rule targets white space as a structuring cue, so it applies only when spacing is doing visible organizational work.

## Tradeoffs of spacing adjustments <!-- role: costs -->

**Sacrifice:** You may give up some plotting area to preserve readable separation.
**Risk:** Changing spacing too far in either direction creates the same accessibility problem in a different form.
**Mitigation:** Adjust spacing while checking specifically for the two extremes named in the guideline: isolated thin marks and crowded marks.

## Common spacing failures <!-- role: mistakes -->

- **Mistake:** Expanding gaps until interval marks become thin and visually isolated. **Why it fails:** The empty space starts to dominate the chart and weakens perceivable structure.
- **Mistake:** Shrinking gaps until bars, intervals, or labels are crowded together. **Why it fails:** The chart becomes harder to parse and understand visually.

## How to review spacing <!-- role: check -->

**Failure Sign:** The chart shows one of two extremes: thin marks with large gaps, or cramped marks with too little separation.
**Quick Check:** Inspect the chart at its intended viewing size and look specifically for those two spacing failures around interval marks and nearby labels.

## How to fix spacing problems <!-- role: fix -->

- Reduce gaps between interval marks when the marks have become thin slivers.
- Add padding between marks or nearby chart elements when the display feels crowded.
- Rebalance broad layout whitespace and local mark spacing so related elements stay grouped without collapsing together.
