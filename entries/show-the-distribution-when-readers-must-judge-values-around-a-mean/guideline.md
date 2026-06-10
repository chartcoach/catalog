---
id: show-the-distribution-when-readers-must-judge-values-around-a-mean
title: Show the distribution when readers must judge values around a mean
bibliography: references.bib
description: For judging likely values around a summarized quantitative result, prefer
  distribution depictions on charts that would otherwise show only a mean bar to improve
  fidelity and mitigate false within-the-bar inferences for readers making decisions
  from the display.
labels:
- purpose:refine
- basis:empirical
- task:distribute
- chart:bar:avoid
- data:quantitative
- quality:fidelity:use
- lever:encoding
- operator:distribution
---

## Distribution display for plausible values <!-- role: advice -->

Show the underlying distribution when readers need to judge what values may plausibly occur around a mean. For example, when a chart would otherwise show only an average as a rising or falling bar, replace that mean bar with a depiction of the distribution itself instead of making readers infer likely values from the filled bar.

## Why the distribution display works <!-- role: reason -->

The within-the-bar bias appears because the bar creates a closed region on only one side of the mean. A distribution display makes the relevant data structure explicit instead of letting the filled bar imply that one side of the mean contains the data.

**Mechanism:** Showing the distribution removes the misleading cue that values inside the bar are more likely than equally distant values outside it.

**Evidence:** Viewers consistently favored within-bar values over equally distant outside-bar values when reasoning about whether a value belonged to the underlying distribution, and this bias was strong enough to reverse decisions when the same mean was shown with rising versus falling bars [@newmanBarGraphsDepicting2012].

## When this applies <!-- role: context -->

- **User Goal:** Judge which values around a mean are plausible, or make a decision based on that judgment.
- **Task:** Interpret the distribution around a mean rather than only the mean itself.
- **Data:** Quantitative observations that can lie above and below the mean.
- **Chart Setting:** The current design shows only a mean as a bar, with or without error bars, and the chart may remain visible during judgment.
- **Audience:** Readers are making an interpretation or decision from the chart rather than only reading off the average.
- **Success Criterion:** Decisions do not flip simply because one side of the mean lies inside a filled bar.

## When not to use it <!-- role: exceptions -->

**Break it when:** You cannot show the underlying distribution and only need to report the mean itself. **Why:** The source recommends using a point for the mean rather than an asymmetric bar in that case.

## Costs of this change <!-- role: costs -->

**Sacrifice:** You move away from a summary-only mean display to a fuller depiction of the data.
**Risk:** Forcing this rule when a distribution display is not possible can block a simpler mean report.
**Mitigation:** If you cannot show the distribution, fall back to a point mark for the mean rather than a bar.

## Common mistake <!-- role: mistakes -->

**Mistake:** Keep the mean bar and add uncertainty decoration instead of exposing the distribution. **Why it fails:** The within-the-bar bias remained with error bars and during free viewing.

## How to test it <!-- role: check -->

**Failure Sign:** A recommendation to increase versus decrease a value would reverse if the same mean were redrawn as a rising bar versus a falling bar.
**Quick Check:** Mock the same mean once from a lower axis and once from an upper axis; if the two versions suggest different plausible directions, the summary bar is distorting interpretation.
**Stronger Test:** Ask whether equally distant positive and negative values around the mean seem equally likely while the chart is visible.

## What to change <!-- role: fix -->

- Replace the mean bar with a depiction of the underlying distribution.
- Remove the asymmetric filled bar if it is the only cue to the summarized result.
- If a full distribution display is not possible, replace the bar with a point mark for the mean.
