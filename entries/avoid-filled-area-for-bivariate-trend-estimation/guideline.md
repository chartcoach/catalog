---
id: avoid-filled-area-for-bivariate-trend-estimation
title: Avoid filled area encoding when viewers must estimate bivariate trends
bibliography: references.bib
description: For by-eye trend estimation in bivariate charts, avoid filled area encoding
  on quantitative plots with ordered x-values to improve fidelity and mitigate less
  accurate relationship judgments for viewers inferring trends directly from the plotted
  data.
labels:
- purpose:refine
- basis:empirical
- task:trend
- data:quantitative
- quality:fidelity:use
- lever:encoding
- channel:area:avoid
---

## Avoid area fill for trend judgment <!-- role: advice -->

Avoid filled area encoding when the chart’s job is to let viewers estimate a bivariate trend by eye. For example, replace an area chart with a line graph or a scatter plot when viewers need to judge the relationship between two quantitative variables.

## Why area fill hurts trend estimation <!-- role: reason -->

Filled area makes one side of the trend visually heavier than the other. That asymmetry pulls by-eye judgments away from the underlying relationship, so viewers estimate the trend less accurately than when they read only points or a line.

**Mechanism:** Filled area changes the perceived balance of the plotted relationship. This makes the overall trend harder to judge accurately from the visual marks alone.

**Evidence:** In the collated extraction for the correlate task, the line and point designs were tied and both significantly outperformed the area design in accuracy, and the source study explains the area-chart deficit as a within-the-area bias during regression by eye [@zengReviewCollationGraphical2023; @correllRegressionEyeEstimating2017].

## Use when readers must infer the relationship directly <!-- role: context -->

- **User Goal:** Estimate the overall relationship or trend by eye.
- **Task:** Judge correlation or trend from the plotted data rather than from a supplied fitted model.
- **Data:** Two quantitative variables shown as a bivariate plot with ordered x-values.
- **Chart Setting:** A static chart where the visual marks themselves carry the trend judgment.
- **Success Criterion:** More accurate by-eye estimation of the relationship.

## Do not use when trend estimation is not the chart's job <!-- role: exceptions -->

**Break it when:** The chart is not intended to support by-eye estimation of the relationship between the variables. **Why:** The evidence only establishes the drawback of filled area for regression-by-eye accuracy.

## Tradeoffs of removing area fill <!-- role: costs -->

**Sacrifice:** You give up the filled-region form as the main bivariate display.
**Risk:** This rule does not tell you whether to switch to a line graph or a scatter plot; the study found both beat the area chart and did not separate them.
**Mitigation:** Make the first edit the same in either case: remove the filled area before asking viewers to judge the relationship.

## Common failure mode with area fill <!-- role: mistakes -->

**Mistake:** Keep the filled area and assume viewers will read the relationship as accurately as they would from a line or points. **Why it fails:** The filled-area design was less accurate for the correlation-style task than both the line and point designs.

## Check whether area fill is hurting the chart <!-- role: check -->

**Failure Sign:** Readers must infer trend or relationship from a chart whose main mark is a filled area under a boundary line.
**Quick Check:** If the chart asks for by-eye trend judgment and uses area fill, flag it for revision.
**Stronger Test:** Render the same data as a line graph or scatter plot and compare the versions in review; prefer the non-area version when accurate trend judgment is the goal.

## Fix the filled-area problem <!-- role: fix -->

- Remove the fill and keep the same boundary as a line graph.
- Replace the area chart with a scatter plot if the plotted points are the primary evidence for the relationship.
- Re-run the trend-reading review on the non-area version after the edit.
