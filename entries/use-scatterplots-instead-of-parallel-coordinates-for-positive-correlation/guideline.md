---
id: use-scatterplots-instead-of-parallel-coordinates-for-positive-correlation
title: Use scatterplots instead of parallel coordinates for positive correlation judgments
bibliography: references.bib
description: For association judgments, prefer scatterplots on bivariate quantitative
  views over parallel coordinates to improve fidelity and address weaker discrimination
  of positive correlations for people comparing relationship strength.
labels:
- purpose:select
- basis:empirical
- task:relate
- chart:scatter:use
- chart:parallel:avoid
- quality:fidelity
- lever:chart-family
- operator:association
---

## Choose the chart family for positive correlation <!-- role: advice -->

Use a scatterplot instead of a parallel-coordinates plot when viewers need to judge the strength of a positive correlation. For example, when the same two quantitative variables could be shown either as a scatterplot or as two connected axes, choose the scatterplot for stronger positive relationships.

## Why the scatterplot works better here <!-- role: reason -->

Positive correlations were judged more precisely in scatterplots than in parallel coordinates. The advantage was specific to the positive-correlation case, not a blanket win across both signs.

**Mechanism:** A scatterplot gave viewers a more discriminable visual pattern for ranking stronger versus weaker positive relationships, while positive parallel-coordinate patterns were harder to separate perceptually.

**Evidence:** Scatterplots depicting positive correlations significantly outperformed parallel coordinates depicting positive correlations, while parallel coordinates depicting negative correlations were not significantly different from scatterplots. The paper fit these judgments with Weber models and used them to rank chart effectiveness for correlation perception [@harrisonRankingVisualizationsCorrelation2014].

**Notes:** This is a bounded contrast for judging correlation strength between two quantitative variables.

## Use when positive-correlation comparison is the job <!-- role: context -->

- **User Goal:** Decide which of two positive relationships is more strongly correlated.
- **Task:** Compare association strength rather than estimate exact numeric correlation.
- **Data:** Two quantitative variables with positive correlation.
- **Chart Setting:** A choice is still open between a scatterplot and a parallel-coordinates view.
- **Success Criterion:** Viewers can reliably tell which relationship is stronger.

## Do not apply this contrast outside the supported sign condition <!-- role: exceptions -->

**Break it when:** The relationship to be judged is negative rather than positive. **Why:** The study found no significant difference between scatterplots and parallel coordinates for negative correlations.

## Costs of switching chart family <!-- role: costs -->

**Sacrifice:** This recommendation only resolves the positive-correlation case.
**Risk:** Applying it as a blanket rule for both positive and negative relationships can overstate the scatterplot advantage.
**Mitigation:** Separate positive and negative relationships before choosing between these two chart families.

## Common failure mode in this comparison <!-- role: mistakes -->

**Mistake:** Treat positive and negative correlations as interchangeable when choosing between scatterplots and parallel coordinates. **Why it fails:** The performance difference depended on the sign of the correlation.

## How to test the choice <!-- role: check -->

**Failure Sign:** Reviewers hesitate or disagree when asked which of two positive relationships is more strongly correlated in a parallel-coordinates view.
**Quick Check:** Render the same positive pair both as a scatterplot and as parallel coordinates, then ask reviewers which version makes the stronger relationship easier to identify.
**Stronger Test:** Use repeated paired comparisons of slightly stronger and weaker positive correlations and keep the version that yields more consistent correct choices.

## What to change <!-- role: fix -->

- Replace the positive-correlation parallel-coordinates view with a scatterplot.
- If the parallel-coordinates form must stay, treat it as a weaker option for positive-correlation judgment and test an alternative layout separately.
- Split positive and negative relationships before standardizing one chart family for both.
