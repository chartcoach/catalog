---
id: place-the-most-important-area-on-the-baseline
title: Place the most important area on the baseline and highlight it with color
bibliography: references.bib
description: For multi-series area charts over ordered time, use baseline order on
  the stacked areas to improve readability and mitigate hard comparisons for readers
  following one key series.
labels:
- purpose:refine
- basis:heuristic
- time:ordered-time
- chart:area
- quality:readability:use
- lever:scale-order
- polish:focus
- channel:color-hue:use
---

## Reorder the stack around the key series <!-- role: advice -->

Move the most important series to the bottom of the stacked area chart and make it stand out with color. For example, place the key area on the shared baseline instead of the middle of the stack, then give that area a distinct color treatment.

## Why the baseline matters <!-- role: reason -->

The bottom area has a stable baseline that readers can compare more easily over time. Color then directs attention to that same series.

**Mechanism:** Putting the key series on the common baseline makes its changes easier to compare, while color helps readers find it quickly.

**Evidence:** The source recommends bringing the most important value to the bottom of the chart and using color to make it stand out, because readers can compare values more easily when they share the same baseline [@muth_area_charts_2018].

## Use when one series deserves emphasis <!-- role: context -->

- **User Goal:** Help readers follow one especially important series in a stacked area chart.
- **Task:** Compare that series over time as easily as possible.
- **Data:** Multiple stacked values over time.
- **Chart Setting:** A stacked area chart with one series that matters most.
- **Audience:** Readers who need to track the key series quickly.
- **Success Criterion:** The key series is easy to find and compare across time.

## Do not use when there is no key stacked series <!-- role: exceptions -->

**Break it when:** The chart has only one value or no clearly most important series to emphasize. **Why:** The source’s benefit comes from giving one key series the shared baseline and extra emphasis.

## What you give up <!-- role: costs -->

**Sacrifice:** You give up whatever previous stack order the chart used.
**Risk:** Other series may become less prominent after the reorder.
**Mitigation:** Use the color emphasis on the key series intentionally, not on several series at once.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Leaving the key series in the middle or at the top of the stack. **Why it fails:** The series then sits on a moving baseline and becomes harder to compare over time.

## How to test the revision <!-- role: check -->

**Failure Sign:** The most important series starts from a changing baseline rather than the bottom of the chart.
**Quick Check:** Reorder the stack so the key series is on the baseline and compare whether it becomes easier to follow.
**Stronger Test:** If the key series is the one readers should compare over time, it should be the series with the shared baseline.

## What to change <!-- role: fix -->

- Move the most important area to the bottom of the stack.
- Apply a standout color to that same area.
- Leave less important areas in less prominent positions and colors.
