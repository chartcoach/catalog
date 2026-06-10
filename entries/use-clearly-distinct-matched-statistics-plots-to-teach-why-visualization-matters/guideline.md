---
id: use-clearly-distinct-matched-statistics-plots-to-teach-why-visualization-matters
title: Use clearly distinct matched-statistics plots to teach why visualization matters
bibliography: references.bib
description: For teaching or explanation, use a multi-view set of plots with matched
  summary statistics to improve insight and mitigate the belief that one statistical
  summary is sufficient for readers learning from example data.
labels:
- purpose:refine
- basis:empirical
- task:compare
- structure:multi-view:use
- quality:insight
- lever:layout-structure
- communication:framing
---

## Matched-statistics example set <!-- role: advice -->

Use a small set of plots that share the same summary statistics but differ clearly in visible structure when you need to demonstrate why data should be visualized. For example, keep the same mean, standard deviation, and correlation, or keep the same median, IQR, and rank correlation, while making one plot look linear, another curved, another outlier-driven, or another shape-based.

## Why the example set works <!-- role: reason -->

The teaching effect comes from a visible conflict between the numbers and the plots. Readers can directly compare panels and see that the same summaries do not guarantee the same pattern.

**Mechanism:** A multi-view set of clearly different plots makes the limits of summary statistics concrete by holding the numbers fixed while changing the visible structure.

**Evidence:** The paper argues that Anscombe-like examples are effective because the plots are clearly different and identifiably distinct, and contrasts them with an unstructured matched-statistics quartet that it describes as not nearly as effective for demonstrating the importance of graphical representations [@matejkaSameStatsDifferent2017].

## When this applies <!-- role: context -->

- **User Goal:** Teach, persuade, or stress-test the claim that summary statistics are sufficient.
- **Task:** Compare several plots that intentionally share the same reported statistics.
- **Data:** Example datasets constructed to preserve chosen summary measures across panels.
- **Chart Setting:** A multi-panel figure, lecture slide, article figure, or explainer.
- **Audience:** Readers are learning why graphical representations matter.
- **Success Criterion:** Each panel is recognizably different while the chosen statistics remain matched.

## When not to use this form <!-- role: exceptions -->

**Break it when:** The individual panels have no obvious structure and are not clearly different from one another. **Why:** The paper explicitly notes that an unstructured matched-statistics set is much less effective as a demonstration.

## Tradeoffs of the example set <!-- role: costs -->

**Sacrifice:** You spend more effort constructing the example than showing one ordinary plot.
**Risk:** If the shaped outputs are poor, points can clump or the result can become undesirable.
**Mitigation:** Use simpler target patterns with better coverage of the coordinate space.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Build a matched-statistics set whose panels are random-looking or too similar to each other. **Why it fails:** The comparison loses its teaching value when readers cannot immediately see distinct structures.

## How to test the example set <!-- role: check -->

**Failure Sign:** The panels share the same statistics, but the visual contrast is weak.
**Quick Check:** Ask whether each panel has an identifiable structure such as a line, curve, outlier pattern, or other recognizable shape.
**Stronger Test:** Compare the set against an unstructured alternative and keep the version with clearer panel-level differences.

## What to change <!-- role: fix -->

- Replace vague or random-looking panels with plots that have clearly identifiable structures.
- Prefer simpler target patterns with broader coverage when shaping the points.
- Reject clumped or weakly differentiated outputs and regenerate until the panels are visibly distinct.
