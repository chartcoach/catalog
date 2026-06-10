---
id: depict-means-with-points-instead-of-bars
title: Depict means with points instead of bars
bibliography: references.bib
description: For reporting a mean in a single summarized quantitative result, avoid
  bar encoding on charts depicting averages to improve fidelity and mitigate within-the-bar
  misinterpretation for readers who may infer likely values from the display.
labels:
- purpose:refine
- basis:empirical
- scope:single-result
- chart:bar:avoid
- data:quantitative
- quality:fidelity:use
- lever:encoding
---

## Point mark for the mean <!-- role: advice -->

Replace the bar mark with a point mark when the chart encodes a mean. For example, show the mean as a point rather than as the endpoint of a rising or falling bar, and do not rely on added error bars to make the bar safe to interpret.

## Why the point mark works <!-- role: reason -->

A mean is symmetric around values above and below it, but a bar is not. The filled bar behaves like a visual object that appears to contain values on one side of the mean, so readers give those within-bar values more weight than equally distant values on the other side.

**Mechanism:** A point mark locates the mean without creating a one-sided enclosed region that readers may treat as containing the underlying data.

**Evidence:** Across six experiments, viewers judged values inside a mean bar as more likely than equally distant values outside it; the effect held with and without error bars, with bars rising from below or falling from above, from memory and during free viewing, and it also changed downstream decisions [@newmanBarGraphsDepicting2012].

## When this applies <!-- role: context -->

- **User Goal:** Report an average and let readers interpret what values around that average are plausible.
- **Task:** Read a mean correctly without biasing one side of the mean.
- **Data:** Quantitative values summarized by a mean.
- **Chart Setting:** A static chart would otherwise depict the mean as a bar from a lower or upper axis, with or without error bars.
- **Audience:** Readers may be students, adults, or general viewers rather than trained statistical specialists.
- **Success Criterion:** Readers treat equally distant values above and below the mean as equally plausible.

## When not to use it <!-- role: exceptions -->

**Break it when:** The value being depicted is inherently asymmetric, such as a count, range, or measure of extremity. **Why:** The source recommends bar graphs for quantities whose meaning is genuinely one-sided.

## Costs of this change <!-- role: costs -->

**Sacrifice:** You depart from a ubiquitous convention for reporting averages.
**Risk:** Applying this rule to inherently asymmetric quantities removes a form that matches the data's one-sided meaning.
**Mitigation:** Keep bars for counts, ranges, or measures of extremity.

## Common mistake <!-- role: mistakes -->

**Mistake:** Add error bars to a mean bar and keep the bar as the main mark. **Why it fails:** The within-the-bar bias persisted both with and without error bars.

## How to test it <!-- role: check -->

**Failure Sign:** One equally distant candidate value would fall inside the filled bar and the matching value on the other side would fall outside it.
**Quick Check:** Ask whether flipping the same mean from a rising bar to a falling bar would change which side of the mean feels more likely.
**Stronger Test:** Show two values equally distant above and below the mean while the chart is visible; if the within-bar value seems more likely, the encoding is misleading.

## What to change <!-- role: fix -->

- Replace the mean bar with a point mark located at the mean.
- Remove the filled bar body when it serves only to connect the mean to an axis.
- If readers need to reason about likely values around the mean, show the distribution instead of a one-sided mean bar.
