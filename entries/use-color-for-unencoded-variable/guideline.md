---
id: use-color-for-unencoded-variable
title: Map color to the variable that position does not already encode
bibliography: references.bib
description: For choosing a color encoding in an already-positioned chart, use color
  on the variable not already mapped to position to improve readability and mitigate
  redundant encoding for readers matching marks to data.
labels:
- purpose:refine
- basis:heuristic
- quality:readability
- lever:encoding
- aesthetic:color:use
---

## Assign color to the unencoded variable <!-- role: advice -->

Map color to the variable that position does not already encode. For example, on a choropleth use fill color for the measured rate rather than for the named region, and on a multi-series line chart use color to distinguish the series because vertical position already shows the value.

## Why this mapping works <!-- role: reason -->

Color works best when it complements, rather than repeats, the chart's positional encoding. Readers can then use position for one variable and color for the other instead of decoding the same field twice.

**Mechanism:** When color carries the variable that position does not already show, each channel answers a different question instead of duplicating the same answer.

**Evidence:** The article's map example colors the rate because geography already identifies the region, and its line-chart example colors the series because vertical position already shows the value [@muth_which_color_scale_2021].

## Use when position already does part of the work <!-- role: context -->

- **User Goal:** Identify both what each mark is and what value it carries.
- **Task:** Match marks to a category or region while also reading a measured value.
- **Data:** One field is already clear from position, and another field still needs visual encoding.
- **Chart Setting:** The chart already uses position to encode one variable, such as geography in a map or value in a line chart.
- **Audience:** Readers scanning the chart to connect marks to data fields.
- **Success Criterion:** Readers can tell both the identity field and the measured field without color repeating position.

## Do not use when color would duplicate position <!-- role: exceptions -->

**Break it when:** Color is assigned to the same variable that position already makes clear. **Why:** The remaining variable stays harder to identify.

## Tradeoffs of this mapping choice <!-- role: costs -->

**Sacrifice:** Color cannot do a second, different job at the same time.
**Risk:** If color repeats the positional field, one important variable is left without a clear color encoding.
**Mitigation:** Decide first which field position already communicates before assigning color.

## Common duplication mistake <!-- role: mistakes -->

**Mistake:** Use color to distinguish regions on a map that already locates each region by position. **Why it fails:** It repeats region identity and misses the chance to encode the measured value with color.

## Check whether color is pulling its weight <!-- role: check -->

**Failure Sign:** The color legend names a field that readers can already identify from position alone.
**Quick Check:** Name what position encodes, then name what color encodes; if both answers are the same field, revise the mapping.
**Stronger Test:** Ask which important field would become unclear if color were removed; if the answer is "none," color is probably duplicating position.

## Fix the color assignment <!-- role: fix -->

- Reassign color to the variable that position does not already encode.
- On maps, use fill color for the measured value when geography already identifies place.
- On multi-series line charts, use distinct series colors for category identity when position already encodes value.
