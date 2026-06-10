---
id: make-independent-y-axis-scales-explicit-in-small-multiples
title: Make independent y-axis scales explicit in small multiples
bibliography: references.bib
description: For small-multiple line charts with independent panel scales, prefer
  explicit scale signaling on the axes and chart description to prevent false cross-panel
  magnitude comparisons and address shared-scale assumptions for readers scanning
  multiple panels.
labels:
- purpose:refine
- basis:heuristic
- structure:small-multiples
- quality:fidelity
- lever:scale-order
- component:axis:use
- communication:context
---

## Flag independent y-axis scales <!-- role: advice -->

Make independent y-axis scales explicit whenever small-multiple panels do not share the same y-axis. For example, note in the chart description that the panel scales differ and use gridlines that look unusual enough to signal that the axes are not shared.

## Why scale differences need a visible warning <!-- role: reason -->

Independent scales change what equal visual height means across panels. Unless that change is clearly signaled, readers can mistake shape comparison for magnitude comparison.

**Mechanism:** Explicit scale signaling forces readers to re-check the axes before comparing panels and reduces false inferences from visually similar heights or slopes.

**Evidence:** The post warns that readers may assume shared y-axes across panels, advises avoiding independent scales when possible, and recommends explicit description text and unusual-looking gridlines when scales differ [@muth_small_multiple_line_charts_2024].

**Notes:** Independent panel scales are also presented as useful when magnitudes differ so much that shared scales hide the trend shape.

## Use when panels need separate scales <!-- role: context -->

- **User Goal:** Show trend shapes despite large magnitude differences across series.
- **Data:** Small-multiple line chart panels that use different y-axis scales.
- **Chart Setting:** Independent panel scales with a risk that readers assume one shared axis.
- **Success Criterion:** Readers notice that scales differ before drawing cross-panel magnitude conclusions.

## Do not use independent scales when shared scales would still work <!-- role: exceptions -->

**Break it when:** Shared y-axis scales are possible without hiding the relevant trends. **Why:** The post recommends avoiding independent scales when possible.

## Costs of independent panel scales <!-- role: costs -->

**Sacrifice:** You give up direct cross-panel magnitude comparability.
**Risk:** Readers may assume a shared scale and draw false insights.
**Mitigation:** Prefer shared scales when possible; otherwise disclose the difference clearly on the chart.

## Common scale-signaling mistake <!-- role: mistakes -->

**Mistake:** Use independent y-axis scales without warning readers. **Why it fails:** Readers may treat the panels as if they share one scale and misread the magnitudes.

## Check whether the scale change is truly visible <!-- role: check -->

**Failure Sign:** The panels look as if they share one y-axis when they do not.
**Quick Check:** If the chart description does not explicitly say the scales differ and the gridlines look normal, readers may miss the scale change.
**Stronger Test:** Ask whether a reader could infer a false cross-panel magnitude comparison from equal visual heights.

## Edits that reveal independent scales <!-- role: fix -->

- Switch to shared y-axis scales if the chart can still show the needed trend differences.
- Add a chart-description note that the y-axis scales differ across panels.
- Use gridlines that do not look like standard shared-scale gridlines.
