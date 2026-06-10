---
id: label-categories-directly-beside-marks
title: Label categories directly beside the marks
bibliography: references.bib
description: For quick category identification in charts with multiple visible categories,
  prefer direct labels on the data marks to improve readability and mitigate repeated
  eye travel for readers scanning between categories and values.
labels:
- purpose:refine
- basis:heuristic
- data:categorical
- quality:readability
- lever:text-annotation
- component:label:use
- component:legend:avoid
---

## Direct labels beside marks <!-- role: advice -->

Label categories next to the marks they describe instead of making readers look back and forth to a separate legend. For example, remove the color key and place series names at the ends of lines or next to pie and donut segments, and add hand-placed annotations when you need extra direct labels.

## Why direct labels reduce eye travel <!-- role: reason -->

Readers understand a chart faster when the explanatory text sits where they need it. A separate legend forces repeated eye movement away from the marks and back again.

**Mechanism:** Direct labels shorten the distance between a category name and its encoded mark, so readers spend less effort matching colors or shapes to meaning.

**Evidence:** The source explicitly recommends removing the color key and labeling categories directly on the chart, with line, pie, and donut charts given as examples and annotations suggested for additional hand-placed labels. [@muth_text_in_data_visualizations_2022]

## Use when category mapping should happen in-chart <!-- role: context -->

- **User Goal:** Identify which mark belongs to which category quickly.
- **Task:** Read category-to-mark mapping without consulting surrounding text.
- **Data:** Multiple categories are distinguished by line, slice, color, or similar marks.
- **Chart Setting:** The chart has enough room to place labels near marks.
- **Audience:** Readers are scanning rather than studying a long explanation first.
- **Success Criterion:** Readers can name each visible category without repeatedly consulting a legend.

## Do not use when space is too tight <!-- role: exceptions -->

**Break it when:** The layout is so tight that labels cannot fit near the marks, especially on mobile. **Why:** The source notes that space can be too constrained for direct labels, so a color key may need to remain at the top.

## Tradeoffs of direct labels <!-- role: costs -->

**Sacrifice:** You give up some plotting space to place labels inside the chart area.\
**Risk:** In a tight layout, direct labels can stop fitting cleanly.\
**Mitigation:** Keep direct labels where they fit, and fall back to a top legend in very tight layouts.

## Common direct-label failure <!-- role: mistakes -->

**Mistake:** Leave category names only in a separate legend or description. **Why it fails:** Readers must keep shifting their eyes away from the marks and may lose the explanation before returning to the data.

## Check label proximity <!-- role: check -->

**Failure Sign:** Readers must repeatedly glance between a legend and the marks to decode categories.\
**Quick Check:** Hide the legend and see whether each visible mark still says what it is.\
**Stronger Test:** Ask whether the category name appears at the mark itself or only somewhere else on the page.

## Fix label placement <!-- role: fix -->

- Remove the legend when the categories can be named directly on the chart.
- Place category names next to the specific lines, slices, or other marks they describe.
- Add annotations by hand when a category needs a direct label that the default layout does not provide.
- Keep a top legend only when the layout is too tight for direct labels.
