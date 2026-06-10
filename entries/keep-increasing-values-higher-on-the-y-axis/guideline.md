---
id: keep-increasing-values-higher-on-the-y-axis
title: Keep increasing values higher on the y-axis
bibliography: references.bib
description: For trend interpretation over ordered time, avoid inverted y-axis order
  on axis-based trend charts to prevent message reversal and mitigate false improvement
  or decline readings for chart readers.
labels:
- purpose:refine
- basis:empirical
- task:trend
- time:ordered-time
- chart:line
- quality:fidelity:use
- lever:scale-order
- component:axis
---

## Y-axis direction <!-- role: advice -->

Keep the y-axis in the conventional upward-increase direction when showing improvement or decline over time. For example, place larger values higher on the page in a line or line-area chart rather than flipping the y-axis so an increase looks like a decrease.

## Why axis direction matters <!-- role: reason -->

Readers attach meaning to direction. Upward movement suggests increase and downward movement suggests decline, so reversing the y-axis can flip the interpreted message even when the data values are correct.

**Mechanism:** Inverting the axis reverses the directional cue that readers use to infer whether the trend improved or worsened.

**Evidence:** In the inverted-axis experiment, 39 of 40 readers answered correctly with the control chart, while 30 of 38 readers answered incorrectly with the inverted-axis version and interpreted the message in the opposite direction [@pandeyHowDeceptiveAre2015].

## Use when the chart must communicate whether a trend improved or declined <!-- role: context -->

- **User Goal:** Decide whether a quantity increased or decreased over time.
- **Task:** Interpret the direction of a trend.
- **Data:** Ordered temporal values on an axis-based chart.
- **Chart Setting:** A line or line-area trend display where y-axis order could be reversed.
- **Audience:** Readers relying on directional conventions to read the chart message.
- **Success Criterion:** Readers identify the correct direction of change instead of reversing it.

## Do not apply this outside axis-based trend displays <!-- role: exceptions -->

**Break it when:** The graphic is not an axis-based trend chart. **Why:** This guideline targets message reversal caused by flipping the direction of an axis that viewers read as up/down change.

## Costs of keeping the conventional direction <!-- role: costs -->

**Sacrifice:** You give up stylistic freedom to place higher values lower on the page.
**Risk:** If you invert the axis for effect, readers may reverse the message.
**Mitigation:** Keep the conventional y-axis order in public-facing trend charts where the direction of change is the main message.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Show the correct numbers but leave the y-axis inverted. **Why it fails:** The study presented accurate data on the chart, yet the inverted axis still caused most readers to interpret the trend backward.

## How to review the axis direction <!-- role: check -->

**Failure Sign:** An increasing series visually slopes downward because higher values are placed lower on the page.
**Quick Check:** Inspect the y-axis labels; if larger values appear below smaller values, the chart uses the inversion tested here.
**Stronger Test:** Compare the current chart to a non-inverted version and ask reviewers whether the quantity improved or declined.

## What to change <!-- role: fix -->

- Reverse the y-axis back so larger values appear higher.
- Redraw the same line or line-area chart after restoring the standard axis order.
- Remove the inverted version rather than trying to correct it with labels or numbers alone.
