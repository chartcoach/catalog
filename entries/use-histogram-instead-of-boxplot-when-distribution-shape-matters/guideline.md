---
id: use-histogram-instead-of-boxplot-when-distribution-shape-matters
title: Use a histogram instead of a boxplot when distribution shape matters
bibliography: references.bib
description: For one-dimensional distribution analysis, use a histogram on quantitative
  data to improve fidelity and mitigate the mistake of treating identical boxplots
  as identical distributions for readers comparing shape.
labels:
- purpose:select
- basis:empirical
- task:distribute
- chart:histogram:use
- chart:box-violin:avoid
- data:quantitative
- quality:fidelity
- lever:chart-family
---

## Histogram over boxplot-only summary <!-- role: advice -->

Choose a histogram instead of a boxplot-only summary when the shape of a one-dimensional quantitative distribution matters. For example, use a histogram to distinguish mass shifted left, shifted right, concentrated at the edges, or split across interior positions, because those distributions can share the same quartiles and whisker limits and still produce identical boxplots.

## Why the histogram works <!-- role: reason -->

A boxplot compresses the distribution to a small set of summary positions. A histogram shows where values accumulate across the range, so readers can distinguish shapes that collapse to the same quartiles and whiskers.

**Mechanism:** The histogram preserves visible distribution shape across bins, while the boxplot hides many different shapes behind the same median, quartiles, and whisker endpoints.

**Evidence:** The paper presents six different one-dimensional distributions with identical first quartile, median, third quartile, and 1.5 IQR whisker locations, and shows that all six produce the same boxplot despite visibly different distributions [@matejkaSameStatsDifferent2017].

## When this applies <!-- role: context -->

- **User Goal:** Compare or explain distribution shape.
- **Task:** Distinguish where values concentrate along a quantitative range.
- **Data:** One quantitative variable.
- **Chart Setting:** The current design relies on a Tukey boxplot as the main summary.
- **Audience:** Readers need to compare shape, not only quartiles and whisker limits.
- **Success Criterion:** Readers can see whether the data are left-heavy, right-heavy, edge-heavy, or distributed across multiple interior regions.

## When a boxplot is enough <!-- role: exceptions -->

**Break it when:** The intended message is only the median, quartiles, and whisker locations. **Why:** Those are exactly the statistics the boxplot is designed to show, and they are the values held constant across the paper's example distributions.

## Tradeoffs of the histogram <!-- role: costs -->

**Sacrifice:** You lose the very compact quartile-and-whisker summary of a boxplot.
**Risk:** If you show only the histogram, readers may not get the exact boxplot summary values directly.
**Mitigation:** Keep the boxplot as a companion view when those summary positions still matter.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Use identical boxplots as evidence that the underlying distributions are similar. **Why it fails:** Different distributions can collapse to the same quartiles and whisker endpoints.

## How to test the choice <!-- role: check -->

**Failure Sign:** Several plausible shapes would produce the same boxplot.
**Quick Check:** Compare a boxplot-only view against a histogram of the same variable; if the histogram reveals distinct shape patterns that the boxplot does not, choose the histogram.
**Stronger Test:** Check whether different candidate distributions share the same quartiles and whisker limits before relying on the boxplot alone.

## What to change <!-- role: fix -->

- Replace the boxplot-only display with a histogram when the message depends on shape.
- Add a histogram beside the boxplot when both shape and quartile summary matter.
- Review where the mass sits along the range instead of inferring shape from the box and whiskers alone.
