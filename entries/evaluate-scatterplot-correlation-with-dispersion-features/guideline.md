---
id: evaluate-scatterplot-correlation-with-dispersion-features
title: Evaluate scatterplot correlation readability with dispersion-based visual features
bibliography: references.bib
description: For correlation comparison, prefer encoding review criteria on scatterplots
  to improve fidelity and address misleading association judgments for designers by
  inspecting dispersion-based visual features rather than Pearson correlation alone.
labels:
- purpose:refine
- basis:empirical
- task:relate
- chart:scatter
- quality:fidelity
- lever:encoding
- operator:association
- audience:designer
---

## Dispersion-based review <!-- role: advice -->

Evaluate scatterplot revisions against the visual features people use to judge correlation, not just the underlying Pearson r. For example, inspect whether perpendicular spread around the implicit trend, prediction-ellipse area, minor-axis length, and confidence-box width remain clearly separated across versions before accepting a redesign for correlation reading.

## Why dispersion cues work <!-- role: reason -->

Correlation judgment in scatterplots follows a small set of visible point-cloud cues rather than the abstract statistic alone. When a redesign preserves separation in those cues, readers are more likely to distinguish nearby correlation levels as intended.

**Mechanism:** Readers appear to use visible dispersion around the regression direction as a proxy for association strength, so designs that preserve those cues support more accurate correlation judgments.

**Evidence:** Across 44 tested visual features, four dispersion-based features predicted judgment correctness better than correlation itself, and models built from those features matched or exceeded existing correlation-based perceptual models for scatterplots [@yangCorrelationJudgmentVisualization2019].

**Notes:** The strongest features all describe dispersion around the regression direction.

## Use when reviewing correlation readability <!-- role: context -->

- **User Goal:** Improve or compare scatterplot designs for accurate reading of association strength.
- **Task:** Judge which of two scatterplots is more correlated, or audit a redesign for that task.
- **Data:** Bivariate quantitative data rendered as a point cloud.
- **Chart Setting:** Scatterplots, including side-by-side comparisons, where viewers infer correlation from the plotted points.
- **Audience:** Designers or reviewers evaluating correlation readability.
- **Success Criterion:** Readers can discriminate nearby correlation levels more reliably.

## Do not generalize beyond this task and chart <!-- role: exceptions -->

**Break it when:** The chart is not a scatterplot or the task is not judging correlation. **Why:** The evidence only establishes these cues for correlation discrimination in scatterplots, not for other chart families or other analytic tasks.

## What this review step costs <!-- role: costs -->

**Sacrifice:** A single-number review based only on Pearson r is no longer enough.\
**Risk:** Checking only one cue can miss how some viewers judge correlation, because the results suggest several visual features may be used.\
**Mitigation:** Inspect the small set of top-performing dispersion cues together instead of relying on one proxy.

## Common review failure <!-- role: mistakes -->

**Mistake:** Accept a scatterplot revision because the data have the intended r values without checking the visible point-cloud features. **Why it fails:** Judgment correctness tracked dispersion-based features more closely than correlation alone.

## How to test the revision <!-- role: check -->

**Failure Sign:** Two versions with different intended correlation readability still look similarly wide or similarly compact around the trend.\
**Quick Check:** Compare candidate versions on perpendicular spread, prediction-ellipse area, minor-axis length, and confidence-box width.\
**Stronger Test:** Model observed judgments with those features and verify that the feature-based fit matches or exceeds the correlation-only baseline.

## What to change next <!-- role: fix -->

- Add the four top-performing dispersion cues to the review checklist for correlation-focused scatterplots.
- Recompute or reinspect those cues after every encoding change that alters the point cloud.
- Reject a revision when it improves the numeric correlation contrast but weakens visible separation in those dispersion cues.
