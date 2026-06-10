---
id: draw-outliers-separately-from-density-context
title: Draw outliers separately from the density context
bibliography: references.bib
description: For outlier inspection in uncertain multivariate plots, use a separate
  outlier layer on density plots to improve insight and address the loss of unusual
  values in PDF summaries for viewers scanning focus and context.
labels:
- purpose:refine
- basis:empirical
- lever:encoding
- operator:uncertainty
- shape:outlier-rich
- quality:insight
---

## Separate outlier layer <!-- role: advice -->

Keep the density plot as context, then render detected outliers in a separate discrete layer. For example, find small isolated regions in pairwise histograms or PDFs, label distributions that predominantly occupy those islands as outliers, and draw those outliers as points or lines apart from the PDF.

## Why a separate outlier layer works <!-- role: reason -->

Density plots emphasize the most likely values, so unusual values can disappear unless they are explicitly surfaced. A separate outlier layer restores focus without discarding the density context, and it naturally avoids overpromoting broad uncertain values.

**Mechanism:** The density layer preserves the overall structure of the data. The outlier layer highlights only samples whose probability mass is concentrated in small isolated regions, so broad uncertain distributions are not mistaken for meaningful outliers.

**Evidence:** The paper notes that density plots de-emphasize outliers, recommends using histogram- or PDF-based outlier detection to identify small isolated regions, and suggests drawing those outliers separately so the display combines focus with context while respecting uncertainty [@fengMatchingVisualSaliency2010].

## When to use a separate outlier layer <!-- role: context -->

- **User Goal:** Inspect unusual values without losing the overall density pattern.
- **Task:** Find and review outliers in uncertain multivariate data.
- **Data:** Uncertain multivariate samples with pairwise histograms or PDFs available for outlier analysis.
- **Chart Setting:** Density-based scatter plots or parallel coordinates where the main density summary hides rare values.
- **Audience:** Analysts or domain experts scanning for unusual cases.
- **Success Criterion:** Small isolated outliers remain visible, while broad uncertain clusters do not gain undue emphasis.

## When a separate outlier layer fails <!-- role: exceptions -->

**Break it when:** The apparent outliers have large variances or spread over a wide range of values instead of fitting within small isolated density islands. **Why:** They are not confidently interesting outliers under the PDF.

## Tradeoffs of a separate outlier layer <!-- role: costs -->

**Sacrifice:** You add another visual layer to the chart.
**Risk:** Too many highlighted marks can compete with the density context.
**Mitigation:** Elevate only distributions that predominantly fall within small isolated regions.

## Common mistake with a separate outlier layer <!-- role: mistakes -->

**Mistake:** Treat every low-density mean as an outlier and draw it discretely. **Why it fails:** Large uncertain distributions can look extreme by mean location even when their probability mass is not isolated.

## How to check a separate outlier layer <!-- role: check -->

**Failure Sign:** A highlighted outlier has broad uncertainty and no clearly isolated density island.
**Quick Check:** Inspect whether the highlighted sample's distribution fits mostly inside a small disconnected region of the histogram or PDF.
**Stronger Test:** Confirm that the highlighted outlier set remains small and isolated relative to the main density mass.

## How to fix a separate outlier layer <!-- role: fix -->

- Run outlier detection on pairwise histograms or PDFs rather than on means alone.
- Highlight only distributions that predominantly occupy small isolated density regions.
- Draw accepted outliers as discrete marks on top of the density plot instead of brightening the full low-density field.
- Leave broad uncertain values in the density context rather than promoting them as outliers.
