---
id: use-bar-chart-instead-of-pie-for-part-comparison
title: Use a bar chart instead of a pie chart for part comparisons
bibliography: references.bib
description: For part-to-whole comparison, use a common-scale bar chart on quantitative
  shares to improve judgment fidelity and mitigate angle-based comparison errors for
  readers making visual estimates.
labels:
- purpose:select
- basis:empirical
- chart:bar:use
- chart:pie-donut:avoid
- quality:fidelity
- lever:chart-family
- operator:part-whole
---

## Common-scale bars <!-- role: advice -->

Replace the pie with bars on a common scale when the task is to compare part sizes. For example, show each part as a bar rather than a wedge, and put the bar scale in percentages or another simple fraction of the whole.

## Why common-scale bars work <!-- role: reason -->

Bars let readers compare part sizes by position along a shared axis. Pie slices force angle and area judgments, so ordering parts and estimating ratios is less reliable.

**Mechanism:** Position on a common scale supports more accurate quantitative judgments than angle. That makes it easier to see both the order of parts and how large one part is relative to another.

**Evidence:** The paper's position-angle experiment found position judgments on bars substantially more accurate than angle judgments on pie charts, and its redesign example shows the same part-whole data becoming easier to order once wedges are replaced by marks on a common scale [@clevelandGraphicalPerceptionTheory1984].

## Use when comparing parts of a whole <!-- role: context -->

- **User Goal:** Compare which parts are larger and by how much.
- **Task:** Make visual ratio judgments or rank the parts of one whole.
- **Data:** Quantitative parts that sum to a whole.
- **Chart Setting:** You are choosing between a pie chart and a bar-based display.
- **Audience:** Readers making quick visual estimates.
- **Success Criterion:** More accurate part comparisons and clearer part ordering.

## Do not use when the chart is not for quantitative part comparison <!-- role: exceptions -->

**Break it when:** The display is not meant to support visual comparison of quantitative parts within a whole. **Why:** The source supports this substitution specifically for judging relative part magnitudes.

## Tradeoffs of replacing the pie <!-- role: costs -->

**Sacrifice:** The display no longer uses a circular whole.
**Risk:** If the bar scale is not expressed as a fraction of the whole, the whole can feel less explicit.
**Mitigation:** Use a 0-100 scale, or another simple fraction scale such as 0-25 or 0-50, so each bar still reads as a share of the whole.

## Common failure with part comparisons <!-- role: mistakes -->

**Mistake:** Keep wedges because the chart already "shows parts of a whole." **Why it fails:** The comparison still depends on angle and area judgments, so part ordering and percent-of-larger estimates stay hard.

## Check the comparison directly <!-- role: check -->

**Failure Sign:** Readers hesitate when asked which part is larger or what percent one part is of another.
**Quick Check:** Render the same values as a pie and as bars, then ask for the part order or a percent-of-largest estimate.
**Stronger Test:** Keep the version that yields quicker and more accurate visual estimates; for this contrast, that is the bar version.

## Fix the display <!-- role: fix -->

- Replace each wedge with one bar on a shared baseline.
- Express the bar scale in percent or another simple fraction of the whole.
- Remove the pie when the chart must support ordering or ratio judgments between parts.
