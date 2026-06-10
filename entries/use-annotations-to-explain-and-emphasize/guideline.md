---
id: use-annotations-to-explain-and-emphasize
title: Use annotations to explain and emphasize chart elements
bibliography: references.bib
description: For explanatory charts and maps, use annotations on chart elements and
  notable data points to improve insight and address missed context for readers following
  the intended message.
labels:
- purpose:refine
- basis:heuristic
- quality:insight
- lever:text-annotation
- component:annotation:use
- communication:context
- polish:annotation
---

## Explanatory annotations <!-- role: advice -->

Add annotations to explain chart elements, point readers to notable data, and supply missing context inside the visualization. For example, annotate a highlight range or connecting line, call out an outlier or important series, and note an external event that explains why values change.

## Why annotations guide interpretation <!-- role: reason -->

Readers get more from an explanatory chart when the important cues and explanations sit inside the chart itself. Small notes also create visual entry points that draw attention to meaningful parts of the display.

**Mechanism:** Annotations turn the chart into a guided reading surface by naming what matters, why it matters, and how to interpret unusual values or added design elements.

**Evidence:** The source calls annotations an extremely powerful tool, says explanatory charts and maps will likely be better with them, and gives examples of annotating highlight ranges, connecting lines, outliers, and events that explain value changes. [@muth_text_in_data_visualizations_2022]

## Use when the chart is meant to guide the reader <!-- role: context -->

- **User Goal:** Understand the intended takeaway, not just inspect raw values.
- **Task:** Notice the important mark, unusual point, or explanatory context within the chart.
- **Chart Setting:** The chart or map contains a highlight, unusual data point, or contextual fact that affects interpretation.
- **Audience:** Readers benefit from pointers to what they should notice.
- **Success Criterion:** The intended point is visible and understandable from the chart itself.

## Do not use when nothing needs explanation or emphasis <!-- role: exceptions -->

**Break it when:** There is no specific chart element to explain, no data point to emphasize, and no contextual fact needed for interpretation. **Why:** The source presents annotations as targeted pointers and explanations, not filler text.

## Tradeoffs of annotations <!-- role: costs -->

**Sacrifice:** You use space that could otherwise stay empty.\
**Risk:** On small screens, the least important annotations may not fit cleanly.\
**Mitigation:** Hide the least important annotations on mobile or move them below the visualization.

## Common annotation failure <!-- role: mistakes -->

**Mistake:** Leave a highlight, outlier, or explanatory event unannotated and expect readers to infer its importance alone. **Why it fails:** Readers get less guidance about what they should notice and why it matters.

## Check annotation coverage <!-- role: check -->

**Failure Sign:** A deliberate highlight, drawn line, outlier, or sharp change appears without on-chart explanation.\
**Quick Check:** Scan the chart and ask whether each intentional emphasis is named where it appears.\
**Stronger Test:** Read the chart without surrounding article text and see whether the intended message still comes through.

## Fix annotation coverage <!-- role: fix -->

- Add a note to any highlight range, connecting line, or other non-data graphic element that needs explanation.
- Add a callout to the data point or series readers should notice first.
- Add brief context where outside events explain a pattern or change in the data.
- Remove or move the least important annotations when small screens cannot support them all.
