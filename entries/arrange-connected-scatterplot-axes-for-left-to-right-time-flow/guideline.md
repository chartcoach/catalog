---
id: arrange-connected-scatterplot-axes-for-left-to-right-time-flow
title: Arrange connected-scatterplot axes so time flows left to right
bibliography: references.bib
description: For trend communication in ordered-time paired series, use left-to-right
  axis ordering on connected scatterplots to improve readability and mitigate time-reversal
  mistakes for novice readers.
labels:
- purpose:refine
- basis:empirical
- task:trend
- time:ordered-time
- chart:scatter
- quality:readability
- lever:scale-order
- literacy:novice
---

## Arrange axes for left-to-right flow <!-- role: advice -->

Arrange the two variables so the connected path progresses globally from left to right across the plot. For example, swap which series is on the x- or y-axis when the main sequence would otherwise run right to left in a static connected scatterplot.

## Why left-to-right flow works <!-- role: reason -->

Readers bring a strong left-to-right expectation for visual exploration and for imagined temporal sequences. When a connected scatterplot violates that expectation, they can reverse the story of the data even if they understand the axes and the points.

**Mechanism:** Left-to-right flow aligns the path with common reading and sequence habits, so readers are less likely to infer the wrong temporal order.

**Evidence:** In the translation study, temporal order was reversed in connected-scatterplot tasks, including simple copying and translation to and from dual-axis line charts; the paper recommends a left-to-right global flow of time to minimize this error in static graphics [@harozConnectedScatterplotPresenting2016].

## Use when left-to-right time flow matters <!-- role: context -->

- **User Goal:** Explain how two measures change over time.
- **Task:** Help readers follow the sequence of a paired time series correctly.
- **Data:** Two simultaneous time series sampled at the same times.
- **Chart Setting:** A static connected scatterplot in print or another non-animated setting.
- **Audience:** Readers who are unfamiliar with connected scatterplots.
- **Success Criterion:** Readers identify the start-to-end order without reversing time.

## Do not use when motion already guides sequence <!-- role: exceptions -->

**Break it when:** The chart is interactive or animated and the motion itself guides viewers through a non-conventional reading direction. **Why:** The paper notes that interaction and animation on the web can help guide sequence reading when the path does not follow the usual left-to-right convention.

## Costs of forcing left-to-right flow <!-- role: costs -->

**Sacrifice:** You may need to place a variable on a less natural axis to preserve a left-to-right temporal path.\
**Risk:** Left-to-right flow alone does not fully solve direction errors.\
**Mitigation:** Pair the axis arrangement with explicit time-direction cues on the path.

## Common axis-order failure <!-- role: mistakes -->

**Mistake:** Keep a right-to-left main flow because the current variable assignment feels natural. **Why it fails:** Readers can reverse the temporal order even when they are only copying or translating the chart.

## Check time-direction readability <!-- role: check -->

**Failure Sign:** A reader narrates the path backward or points to the wrong start and end.\
**Quick Check:** Ask someone to point to the first and last point and describe the sequence without help from surrounding text.\
**Stronger Test:** Compare the current axis assignment with a version that swaps the two variables and keep the version that produces fewer reversed readings.

## Fix the axis assignment <!-- role: fix -->

- Swap the two variables across the x- and y-axes if that makes the path run more clearly from left to right.
- Recheck the path after the swap and confirm that the main temporal sweep no longer runs backward.
- If you must keep a non-left-to-right path, add explicit time-direction annotation to the line.
