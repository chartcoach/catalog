---
id: use-scatterplot-instead-of-summary-statistics-alone-for-bivariate-data
title: Use a scatterplot instead of summary statistics alone for bivariate data
bibliography: references.bib
description: For bivariate relationship analysis, use a scatterplot on paired quantitative
  data to improve trust and mitigate the mistake of treating equal summary statistics
  as equal structure for readers interpreting associations.
labels:
- purpose:select
- basis:empirical
- task:relate
- chart:scatter:use
- chart:text:avoid
- data:quantitative
- quality:trust
- lever:chart-family
---

## Scatterplot over summary-only report <!-- role: advice -->

Choose a scatterplot instead of a summary-only report when you need to inspect or communicate the relationship between two quantitative variables. For example, plot the point cloud rather than only listing x/y mean, x/y standard deviation, and Pearson or Spearman correlation, because the same values can correspond to a noisy line, a curve, an outlier-driven pattern, a vertical pattern, or a shape-based pattern.

## Why the scatterplot works <!-- role: reason -->

A scatterplot exposes visible structure that summary statistics can leave unchanged. It lets readers see whether the reported association comes from an overall linear pattern, a curve, a single influential point, or some other arrangement.

**Mechanism:** Plotting the individual points reveals form, outliers, and grouped structure that are hidden when readers get only averages, spread measures, and a correlation coefficient.

**Evidence:** The paper shows multiple bivariate datasets with identical summary statistics to two decimal places that nevertheless produce very different scatterplots, and explicitly presents these examples as demonstrations of the importance of visualizing data rather than relying on statistics alone [@matejkaSameStatsDifferent2017].

## When this applies <!-- role: context -->

- **User Goal:** Inspect or explain the association between two variables.
- **Task:** Judge whether the relationship is linear, curved, outlier-driven, vertical, or otherwise patterned.
- **Data:** Paired quantitative observations.
- **Chart Setting:** The current output is a text or numeric summary built from means, spread statistics, and correlation.
- **Audience:** Readers are expected to interpret the relationship from summary values.
- **Success Criterion:** Readers can see the actual point pattern instead of inferring it from a few numbers.

## When not to use the original points <!-- role: exceptions -->

**Break it when:** The point locations themselves cannot be published because the data are sensitive. **Why:** The paper treats confidentialization as a separate use case and discusses replacing the original points with visually similar cloned data instead of publishing the source points.

## Tradeoffs of the scatterplot <!-- role: costs -->

**Sacrifice:** You give up the compactness of a short numeric summary.
**Risk:** A single aggregate scatterplot can still hide subgroup reversals.
**Mitigation:** Inspect subgroup views as well when the data contain meaningful groups.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Treat equal means, spread measures, and correlation as evidence that two bivariate datasets will look the same. **Why it fails:** Very different point arrangements can preserve those statistics while implying different interpretations.

## How to test the choice <!-- role: check -->

**Failure Sign:** A summary-only report suggests a simple relationship, but the scatterplot reveals a different visible structure.
**Quick Check:** Compare the summary-only report against a scatterplot of the same data; if the scatterplot reveals curvature, a vertical pattern, or an outlier-driven relationship, choose the scatterplot.
**Stronger Test:** If the data are grouped, compare the aggregate scatterplot with subgroup views to see whether the overall trend hides different within-group trends.

## What to change <!-- role: fix -->

- Replace the summary-only report with a scatterplot of the individual points.
- Keep the summary statistics only as a companion to the scatterplot, not as the sole representation.
- Separate groups into additional views when one combined scatterplot hides within-group direction.
