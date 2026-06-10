---
id: use-violin-plot-instead-of-mean-bar-with-error-bars
title: Use a violin plot instead of a mean bar chart with error bars when distribution
  matters
bibliography: references.bib
description: For grouped comparisons where distribution shape can change interpretation,
  use a violin plot on grouped results to improve insight and mitigate within-the-bar
  bias for analysts comparing sample populations.
labels:
- purpose:select
- basis:empirical
- task:compare
- scope:grouped-result
- chart:box-violin:use
- chart:bar:avoid
- operator:distribution
- quality:insight
---

## Distribution display <!-- role: advice -->

Use a violin plot instead of a mean bar chart with error bars when readers need to see the data distribution. For example, compare sample groups with violins that show the distribution alongside the mean rather than bars that show only the mean and error.

## Why group summaries need visible distributions <!-- role: reason -->

A mean-only chart hides structure that can change the interpretation of a comparison. Readers can estimate distributional properties visually, but they need the distribution to be shown.

**Mechanism:** A violin plot exposes spread and shape while preserving a summary statistic such as the mean. This avoids the within-the-bar bias that makes values inside a bar seem more likely than values outside it.

**Evidence:** The paper warns that bar charts with error bars can induce within-the-bar bias and recommends violin plots because they show the distribution alongside the mean and reveal patterns such as normal, bimodal, and skewed samples [@szafirGoodBadBiased2018].

## Use when grouped distributions may change the conclusion <!-- role: context -->

- **User Goal:** Compare sample populations without losing distribution shape.
- **Task:** Compare groups on both summary and distribution.
- **Data:** Grouped quantitative samples where variance, density, or shape may matter.
- **Chart Setting:** A grouped comparison has enough space to show more than a single summary bar.
- **Audience:** Analysts or readers who must judge more than the mean.
- **Success Criterion:** Readers can see shape differences such as spread, skew, or multimodality.

## Do not use when only aggregate statistics are needed or the data is too large to show directly <!-- role: exceptions -->

- **Break it when:** Aggregate statistics are sufficient for the analysis. **Why:** The source states that some questions can be addressed with representative statistics alone.
- **Break it when:** The dataset is too large to visualize directly without clutter. **Why:** The source notes that showing everything can overwhelm the display and recommends visual summaries, filtering, or subsampling in that case.

## What you trade away <!-- role: costs -->

**Sacrifice:** You lose the very compact mean-only readout of a bar chart.
**Risk:** Showing more of the data can create clutter, especially with large datasets.
**Mitigation:** Use visual summaries, filtering, or subsampling when the full dataset is too dense to show clearly.

## Common summary failure <!-- role: mistakes -->

**Mistake:** Using bars with error bars as the only display for group comparison. **Why it fails:** Readers overinterpret the filled bar region and cannot see whether groups differ by spread, skew, or multimodality.

## How to choose between the two charts <!-- role: check -->

**Failure Sign:** The chart shows only means and error bars, but the analysis may depend on distribution shape.
**Quick Check:** Compare a mean-bar version and a violin version of the same grouped data; if the violin reveals shape differences that could affect interpretation, keep the violin.
**Stronger Test:** Ask whether a reader can tell if a group is normal, bimodal, or skewed from the current chart alone.

## What to change <!-- role: fix -->

- Replace each mean bar with a violin that shows the distribution.
- Keep the mean visible alongside the violin.
- Remove bar fills that imply the interior is more likely than values outside the bar.
- If the full data is too dense, use visual summaries, filtering, or subsampling before plotting.
