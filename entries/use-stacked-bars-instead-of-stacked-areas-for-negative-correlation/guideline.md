---
id: use-stacked-bars-instead-of-stacked-areas-for-negative-correlation
title: Use stacked bar charts instead of stacked area charts for negative correlation
  judgments
bibliography: references.bib
description: For association judgments, prefer stacked bar charts over stacked area
  charts on negatively correlated quantitative series to improve fidelity and address
  weaker discrimination of correlation strength for people comparing opposite-moving
  values.
labels:
- purpose:select
- basis:empirical
- task:relate
- chart:bar:use
- chart:area:avoid
- quality:fidelity
- lever:chart-family
- operator:association
---

## Choose stacked bars over stacked areas for negative relationships <!-- role: advice -->

Use a stacked bar chart instead of a stacked area chart when viewers need to judge the strength of a negative correlation. For example, if two quantitative series move in opposite directions and you are choosing between these two stacked forms, render them as stacked bars rather than stacked areas.

## Why the stacked bar performs better here <!-- role: reason -->

The stacked forms were not perceptually interchangeable. For negative correlations, stacked bars supported more precise judgments than stacked areas.

**Mechanism:** The stacked bar layout gave viewers a more discriminable pattern for comparing stronger versus weaker negative relationships than the stacked area form.

**Evidence:** For negatively correlated data, stacked bar charts significantly outperformed stacked area charts in correlation-judgment precision, and both were modeled with Weber-style fits after filtering unreliable conditions [@harrisonRankingVisualizationsCorrelation2014].

**Notes:** The paper also reports that viewers appeared to use different visual cues in stacked bars than in stacked areas.

## Use when the sign is negative and the chart family is still open <!-- role: context -->

- **User Goal:** Help viewers compare which negative relationship is stronger.
- **Task:** Judge association strength, not exact values.
- **Data:** Two quantitative series with negative correlation.
- **Chart Setting:** A stacked display is desired and the choice is between stacked bars and stacked areas.
- **Success Criterion:** Viewers can more reliably rank stronger and weaker negative correlations.

## Do not extend this contrast to unsupported sign conditions <!-- role: exceptions -->

**Break it when:** The relationship to be judged is positive rather than negative. **Why:** Positive stacked-area and positive stacked-bar conditions frequently hit the study's chance boundary, so this contrast was not supported for positive correlations.

## Costs of changing the stacked form <!-- role: costs -->

**Sacrifice:** This recommendation only covers the negative-correlation case.
**Risk:** Treating it as a general rule for all stacked relationships can overreach the evidence.
**Mitigation:** Check the correlation sign before deciding between stacked bars and stacked areas.

## Common failure mode in this comparison <!-- role: mistakes -->

**Mistake:** Assume stacked bars and stacked areas are perceptually equivalent because their overall shapes look similar. **Why it fails:** The study found a significant performance difference between them for negative correlations.

## How to test the choice <!-- role: check -->

**Failure Sign:** Reviewers struggle to tell which of two negative stacked-area relationships is more strongly correlated.
**Quick Check:** Render the same negative relationship once as stacked bars and once as stacked areas, then ask which version makes the stronger correlation easier to identify.
**Stronger Test:** Use repeated paired comparisons of slightly different negative correlations and keep the chart type that produces more consistent correct choices.

## What to change <!-- role: fix -->

- Replace the stacked area chart with a stacked bar chart for the negative-correlation view.
- Re-run the comparison on the same data after the swap instead of assuming the stacked forms behave the same.
- If positive and negative relationships both appear in the project, choose chart families for those cases separately.
