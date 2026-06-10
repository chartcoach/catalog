---
id: remove-superfluous-pictographs
title: Remove pictographs that do not encode data
bibliography: references.bib
description: For brief recall and rapid lookup tasks, avoid superfluous imagery on
  simple bar charts to prevent distraction and mitigate slower and less accurate value
  extraction for viewers reading values under time pressure.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- chart:bar
- quality:readability
- lever:encoding
- aesthetic:style:avoid
---

## Superfluous imagery <!-- role: advice -->

Remove pictographs that do not carry data from value charts. For example, keep bars plain instead of placing a large category image behind them, and reserve pictographs for cases where the icons themselves encode the values.

## Why non-data images hurt reading <!-- role: reason -->

A non-data image adds another object to inspect but does not help decode the numbers. That extra picture competes with the bars for attention and memory, so viewers extract the values less efficiently.

**Mechanism:** Removing irrelevant imagery keeps attention on the value marks and reduces interference during both brief recall and speeded value comparison.

**Evidence:** A superfluous background image caused substantially higher recall error than the other chart types in experiment 1, and it was the only chart variant that was slower than the standard bar chart in experiment 4 [@harozISOTYPEVisualizationWorking2015].

## Use when the image is decorative rather than data-bearing <!-- role: context -->

- **User Goal:** Recover exact values or answer a quick value-comparison question.
- **Task:** Brief-glance recall or rapid value lookup.
- **Data:** Small sets of quantitative category values.
- **Chart Setting:** A simple bar-like chart includes a large background or decorative picture that is unrelated to the scale.
- **Audience:** Viewers reading quickly rather than studying the chart at length.
- **Success Criterion:** Lower recall error and faster responses.

## Do not apply this to data-bearing pictographs <!-- role: exceptions -->

**Break it when:** The pictograph is the data mark itself rather than a background decoration. **Why:** The observed costs came from images that did not encode data.

## Tradeoffs of removing decorative imagery <!-- role: costs -->

**Sacrifice:** You give up some ornament and novelty.
**Risk:** The chart may feel less visually distinctive at first glance.
**Mitigation:** If imagery is important, move it into the data marks instead of leaving it as a separate background picture.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Adding a large topical picture behind the bars because it matches the subject. **Why it fails:** The picture does not help read the values and instead makes recall and lookup worse.

## How to test it <!-- role: check -->

**Failure Sign:** Viewers hesitate, mention the background image, or make more value errors than expected.
**Quick Check:** Compare the chart against a version with the background image removed in a brief recall or timed lookup task.
**Stronger Test:** Measure average absolute recall error or response time against the plain bar version.

## What to change <!-- role: fix -->

- Delete the background image or other non-data pictograph.
- Keep only the quantitative marks and necessary labels.
- If you need imagery, convert it into the marks that encode the values instead of leaving it decorative.
