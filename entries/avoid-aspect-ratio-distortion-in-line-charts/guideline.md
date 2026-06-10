---
id: avoid-aspect-ratio-distortion-in-line-charts
title: Avoid aspect-ratio distortion in line charts
bibliography: references.bib
description: For trend reading over ordered time, avoid aspect-ratio distortion on
  line charts to prevent message exaggeration or understatement and mitigate misreading
  of rate of change for chart readers.
labels:
- purpose:refine
- basis:empirical
- task:trend
- time:ordered-time
- chart:line
- quality:fidelity:use
- lever:layout-structure
---

## Line-chart aspect ratio <!-- role: advice -->

Keep the line-chart aspect ratio from artificially flattening or steepening the line. For example, do not widen one axis so the same time-series looks like it changed more slowly or more sharply than it actually did.

## Why aspect ratio matters for trends <!-- role: reason -->

Readers use line angle to judge increase and decrease. Changing the aspect ratio changes that angle without changing the data, so the perceived rate of change becomes stronger or weaker than the underlying trend.

**Mechanism:** Stretching or compressing one axis alters the line's inclination, which changes how quickly the trend appears to rise or fall.

**Evidence:** In the line-chart experiment, the distorted aspect ratio produced much larger "how much did it improve" judgments than the control version (mean 3.19 vs. 1.39 on a 5-point scale; p < 0.0001) [@pandeyHowDeceptiveAre2015].

## Use when the chart must show the real rate of change <!-- role: context -->

- **User Goal:** Judge how much a quantity improved or declined over time.
- **Task:** Read the rate of increase or decrease from the line.
- **Data:** Ordered temporal values shown as a time series.
- **Chart Setting:** A line chart whose axes could be widened or compressed.
- **Audience:** Readers interpreting the chart's trend message directly from the line shape.
- **Success Criterion:** The perceived steepness of the trend matches the underlying data.

## Do not apply this outside line-based rate judgments <!-- role: exceptions -->

**Break it when:** The chart is not a line chart or the message does not depend on perceived increase or decrease rate. **Why:** This guideline targets the distortion created when line angle is used to infer rate, and the paper discusses this distortion primarily for line charts.

## Costs of preserving the undistorted aspect ratio <!-- role: costs -->

**Sacrifice:** You give up some rhetorical control over how dramatic the trend looks.
**Risk:** A real increase may appear less striking than in a stretched version.
**Mitigation:** Keep the undistorted aspect ratio so the visual rate stays aligned with the data.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep the distorted aspect ratio and assume printed values will correct the reading. **Why it fails:** The study used charts that showed the actual data values, yet the altered aspect ratio still changed readers' judgments.

## How to review the aspect ratio <!-- role: check -->

**Failure Sign:** The same data would look much flatter or steeper if one axis were rescaled.
**Quick Check:** Inspect whether one axis has been widened or compressed in a way that changes the line angle without changing the data.
**Stronger Test:** Compare the chart to a control version with the original scales and ask reviewers the same "how much did it improve" question.

## What to change <!-- role: fix -->

- Undo the axis stretching or compression that changes the line angle.
- Redraw the same time series with the control-style aspect ratio.
- Remove the distorted version rather than trying to offset it with numeric labels alone.
