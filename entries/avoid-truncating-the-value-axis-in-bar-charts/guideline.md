---
id: avoid-truncating-the-value-axis-in-bar-charts
title: Avoid truncating the value axis in bar charts
bibliography: references.bib
description: For magnitude comparison, avoid truncating the value axis on bar charts
  to prevent message exaggeration and mitigate overstatement of differences for chart
  readers.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:bar
- data:quantitative
- quality:fidelity:use
- lever:encoding
- component:axis
---

## Value-axis baseline <!-- role: advice -->

Keep the bar-chart value axis untruncated so bar length reflects the actual magnitude difference. For example, show both bars on the full value scale rather than raising the axis minimum to make a small difference look much larger.

## Why the full baseline matters <!-- role: reason -->

Bar length is read against the displayed axis range. When the axis range is shortened, the same data produces a much stronger visual gap, so readers overstate how much larger one value is than another.

**Mechanism:** Truncating the value axis exaggerates the perceived difference while leaving the underlying numbers unchanged, so the visual message becomes stronger than the data.

**Evidence:** In the bar-chart experiment, truncated-axis charts produced much higher "how much bigger" judgments than full-axis charts (mean 2.77 vs. 1.45 on a 5-point scale; p = 0.0003), even though the chart still showed the actual numbers [@pandeyHowDeceptiveAre2015].

## Use when the bar chart must show the real size of a difference <!-- role: context -->

- **User Goal:** Judge how much one category exceeds another.
- **Task:** Compare magnitude, not just direction.
- **Data:** A small set of quantitative category values.
- **Chart Setting:** A bar chart with a visible value axis and a message-level comparison.
- **Audience:** Readers who will interpret the chart visually rather than recalculate from the numbers.
- **Success Criterion:** The perceived size of the difference matches the data instead of an exaggerated visual gap.

## Do not apply this as a special-case rule outside the tested setup <!-- role: exceptions -->

**Break it when:** The graphic is not an axis-based bar chart. **Why:** This guideline targets the exaggeration created by changing the axis range that bar length is read against, and the paper tested that mechanism with bar charts.

## Costs of keeping the full axis <!-- role: costs -->

**Sacrifice:** You give up some visual drama.
**Risk:** A small real difference may look modest.
**Mitigation:** Keep the full axis and let the chart communicate the actual size of the difference rather than amplifying it with the scale.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Show the exact values on the bars but still truncate the value axis. **Why it fails:** The study presented accurate numbers on the chart and readers still gave exaggerated magnitude judgments.

## How to review the bar chart <!-- role: check -->

**Failure Sign:** The bars look far more different than the numeric values suggest.
**Quick Check:** Inspect the displayed minimum on the value axis; if the scale starts above the natural baseline used in the control-style version, the chart uses the distortion tested here.
**Stronger Test:** Compare the current chart to a full-axis version and ask a reviewer the same "how much bigger" question; if the truncated version yields a stronger answer, keep the full-axis version.

## What to change <!-- role: fix -->

- Reset the bar-chart value axis to the full baseline instead of an enlarged segment.
- Redraw the same bars against the unaltered axis range.
- Remove the truncated version rather than trying to offset it with printed numbers alone.
