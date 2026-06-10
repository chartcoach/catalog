---
id: mute-comparison-series-with-grey
title: Mute comparison series and reserve color for the focal series
bibliography: references.bib
description: For comparison tasks in multi-series charts, use muted color on non-focal
  series to improve readability and mitigate split attention for readers when one
  series is the intended focus.
labels:
- purpose:refine
- basis:heuristic
- task:compare
- quality:readability:use
- lever:encoding
- measure:multi
- polish:focus
- aesthetic:color:use
---

## Create color hierarchy between focal and comparison series <!-- role: advice -->

Mute comparison series with grey and reserve a stronger color for the focal series. For example, in a multi-line chart, keep benchmark lines grey and give the single series that carries the main point the accent color.

## Why greyed comparison series work <!-- role: reason -->

Color is one of the fastest ways to direct attention. A muted palette keeps supporting data present without letting it compete for the first look.

**Mechanism:** Grey pushes comparison data into the background while a stronger accent color acts as a spotlight on the series that should lead the reading.

**Evidence:** The post describes color as a spotlight, says grey is especially important when charts contain comparison data, and demonstrates the focal series in color while the comparison series are moved into the background with grey [@muth_better_charts_2017].

## Use when one series should lead the reading <!-- role: context -->

- **User Goal:** Help readers compare several series while still seeing one series as the main one.
- **Task:** Compare a focal series against supporting series.
- **Data:** Multiple encoded series appear in the same chart.
- **Chart Setting:** The extra series are present for comparison, but one series is the star of the show.
- **Success Criterion:** Readers notice the focal series first and can still read the supporting series.

## Do not use it when there is no single star series <!-- role: exceptions -->

**Break it when:** The comparison series are not background context and the chart is not supposed to elevate one series above the others. **Why:** This color hierarchy depends on one series being the intended focus.

## Tradeoffs of strong color hierarchy <!-- role: costs -->

**Sacrifice:** The comparison series become less prominent.
**Risk:** If you mute data that should share the main message, readers may underread them.
**Mitigation:** Reserve the accent color for the single series that is supposed to lead the reading.

## Common color-hierarchy failure <!-- role: mistakes -->

**Mistake:** Give the focal series and the comparison series the same visual prominence. **Why it fails:** Readers lose a clear target for attention and the chart becomes less clean.

## How to check color hierarchy <!-- role: check -->

**Failure Sign:** Several series compete equally for attention.
**Quick Check:** Count the strongly highlighted series. If more than one supporting series has the same emphasis as the focal one, the hierarchy is weak.
**Stronger Test:** Ask a reviewer which series seems most important at first glance. If they do not pick the intended focal series, reduce the color emphasis on the others.

## How to fix color hierarchy <!-- role: fix -->

- Recolor non-focal series in grey.
- Keep the accent color on the single series that carries the main point.
- Remove extra highlight colors from supporting series.
