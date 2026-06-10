---
id: use-scatterplots-instead-of-parallel-coordinates-for-bivariate-correlation-judgment
title: Use a scatterplot instead of parallel coordinates for bivariate correlation
  judgments
bibliography: references.bib
description: For bivariate correlation analysis, use the scatterplot chart family
  over parallel coordinates on paired quantitative variables to improve fidelity and
  address slower, less accurate association judgments for readers estimating direction
  and strength of correlation.
labels:
- purpose:select
- basis:empirical
- task:relate
- chart:scatter:use
- chart:parallel:avoid
- data:quantitative
- quality:fidelity:use
- lever:chart-family
- operator:association
---

## Switch the chart family <!-- role: advice -->

Choose a scatterplot instead of parallel coordinates when the chart’s job is to let readers judge the direction and strength of correlation between two quantitative variables. For example, map the two variables to x and y position in a point plot rather than to two parallel axes connected by line segments when readers must decide whether the relationship is negative, zero, or positive.

## Why the scatterplot works better here <!-- role: reason -->

Correlation judgment depends on reading a bivariate pattern quickly enough to estimate both direction and strength. The scatterplot preserves that pattern in a form readers judged more accurately and more quickly than the parallel-coordinates alternative.

**Mechanism:** Positioning points on x and y axes supports direct reading of association between two quantitative variables, while the parallel-coordinates alternative makes the same relationship harder to judge efficiently in this task.

**Evidence:** In the collated extraction, the scatterplot ranked above the parallel coordinates plot for the correlate task on both accuracy and time, with significant differences reported for each metric [@zengReviewCollationGraphical2023; @liJudgingCorrelationScatterplots2010].

## Use when these conditions are all true <!-- role: context -->

- **User Goal:** Judge the direction and strength of association between two variables.
- **Task:** Correlate.
- **Data:** One paired set of two quantitative variables.
- **Chart Setting:** You are choosing the primary chart form for a single bivariate view.
- **Audience:** Readers need to classify the relationship as weaker or stronger, and as negative, zero, or positive.
- **Success Criterion:** More accurate and faster correlation judgments.

## Do not use when these conditions are true <!-- role: exceptions -->

**Break it when:** The chart is not being used for a single bivariate correlation judgment, or the task is something other than judging correlation. **Why:** The evidence only compares scatterplots and parallel coordinates for the correlate task on one pair of quantitative variables.

## Tradeoffs of this choice <!-- role: costs -->

**Sacrifice:** You give up the parallel-coordinates view as the primary display for this correlation judgment.
**Risk:** If you apply the rule outside a single bivariate correlation-reading task, you may replace a view chosen for other analytic reasons.
**Mitigation:** Limit the switch to the specific view whose main job is judging one correlation.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keeping a parallel-coordinates plot as the main chart for judging one pair’s correlation because both charts can encode the same two variables. **Why it fails:** The parallel-coordinates option produced slower and less accurate judgments in the compared correlate task.

## How to check the decision <!-- role: check -->

**Failure Sign:** Reviewers hesitate, disagree, or take longer when estimating whether the relationship is negative, zero, or positive.
**Quick Check:** Render the same two variables as both a scatterplot and a parallel-coordinates plot, then ask reviewers to judge direction and rough strength; prefer the version that yields faster and more consistent answers.
**Stronger Test:** Time a small review in which readers rate each version on a five-level scale from strong negative to strong positive, then compare completion time and agreement.

## What to change <!-- role: fix -->

- Replot the same two quantitative variables as a scatterplot with one variable on x and the other on y.
- Use the scatterplot as the primary view for the correlation judgment instead of the parallel-coordinates plot.
- If the parallel-coordinates plot must remain for another purpose, add a scatterplot for the specific variable pair readers need to judge.
