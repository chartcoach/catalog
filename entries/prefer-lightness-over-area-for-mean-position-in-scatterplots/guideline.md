---
id: prefer-lightness-over-area-for-mean-position-in-scatterplots
title: Prefer point lightness over point area for mean-position judgments in scatterplots
bibliography: references.bib
description: For summary judgments of x/y mean position, prefer lightness encoding
  over point area on trivariate scatterplots to improve fidelity and mitigate weighted-average
  bias for readers deciding which points fall above or below average.
labels:
- purpose:refine
- basis:empirical
- chart:scatter
- measure:multi
- lever:encoding
- channel:color-saturation:use
- channel:area:avoid
- quality:fidelity:use
---

## Third-variable encoding for mean reading <!-- role: advice -->

Encode the third quantitative variable with point lightness instead of point area when readers must judge the average x/y position of a scatterplot. For example, replace bubble-sized points with equal-sized points that vary in lightness, especially when the chart is used to judge which points lie above or below average.

## Why lightness works better here <!-- role: reason -->

Point area gives visually larger marks extra weight in the perceived center of the point cloud. Lightness can also pull the perceived mean, but the pull is smaller, so readers stay closer to the true x/y average when the third variable is carried by lightness rather than size.

**Mechanism:** Using lightness reduces the amount that visually dominant marks distort the perceived mean position of the scatterplot.

**Evidence:** In the collated experiment, lightness-encoded scatterplots outperformed area-encoded bubble variants on aggregate mean-position judgments across the tested range and correlation conditions, and the underlying study found stronger bias and higher error from size than from lightness for this task [@zengReviewCollationGraphical2023; @hongWeightedAverageIllusion2022].

**Notes:** The improvement is relative, not absolute: darker marks can still pull the perceived mean.

## Use when mean position is the reading target <!-- role: context -->

- **User Goal:** Estimate the overall x/y mean or use that mean as a threshold for above/below-average judgments.
- **Task:** Read a visual summary of the point cloud rather than compare exact third-variable values on individual marks.
- **Data:** Three quantitative variables are shown in one scatterplot.
- **Chart Setting:** A static scatterplot currently uses point area or could use point lightness for the third variable.
- **Audience:** Readers are expected to infer the mean from the marks rather than from an explicit computed summary.
- **Success Criterion:** The perceived center of the cloud stays close to the true x/y mean.

## Do not use when individual size readout matters more <!-- role: exceptions -->

**Break it when:** Reading the third variable on individual marks is more important than judging the overall x/y mean. **Why:** The source notes that size is a more precise channel than lightness for communicating individual values, even though it interferes more with position summaries.

## What you give up by switching channels <!-- role: costs -->

**Sacrifice:** You give up some precision in reading the third variable from individual marks.
**Risk:** Lightness can still bias mean judgments when darker marks cluster with position.
**Mitigation:** Use this revision when the chart's main job is summary reading, then inspect whether darker marks still accumulate on one side of the plot.

## Common failure after the channel swap <!-- role: mistakes -->

**Mistake:** Switching from area to lightness and assuming the summary task is now unbiased. **Why it fails:** Darker points still pull the perceived mean, so the change reduces bias rather than eliminating it.

## How to review the encoding choice <!-- role: check -->

**Failure Sign:** The bubble version makes one side of the cloud look above average mainly because the largest points sit there.
**Quick Check:** Compare the same scatterplot once with point area and once with point lightness; if the perceived center moves farther toward the large-point cluster in the area version, revise.
**Stronger Test:** Ask a reviewer to click the perceived mean on both versions and compare the displacement from the true mean.

## What to change in the chart <!-- role: fix -->

- Remap the third quantitative variable from point area to point lightness.
- Keep point size constant after the remap so the x/y mean is carried by position rather than bubble size.
- Re-check the chart by comparing the perceived mean before and after the remap.
