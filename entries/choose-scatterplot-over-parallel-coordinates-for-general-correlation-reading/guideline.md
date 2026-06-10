---
id: choose-scatterplot-over-parallel-coordinates-for-general-correlation-reading
title: Choose a scatterplot over parallel coordinates for general bivariate correlation
  reading
bibliography: references.bib
description: For relate tasks on bivariate quantitative data, prefer a scatterplot
  over parallel coordinates to improve fidelity and address inconsistent correlation
  reading across positive and negative relationships for broad-use correlation displays.
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

## Scatterplot over parallel coordinates <!-- role: advice -->

Use a scatterplot as the default chart family for reading the strength of association between two quantitative variables. For example, when the same workflow may need to show either positive or negative correlation, use a scatterplot instead of parallel coordinates as the general-purpose correlation view.

## Why this choice works <!-- role: reason -->

A scatterplot stays precise when readers judge both positive and negative relationships, so one chart family can cover the full sign range without changing the reader's interpretation strategy. Parallel coordinates stay competitive for negative correlation, but they do not keep the same performance across both signs.

**Mechanism:** A scatterplot gives one consistent positional view of both variables, which supports more stable correlation judgments across datasets that may slope upward or downward.

**Evidence:** The collated result places scatterplots in the top JND group for correlation judgment, and the re-analysis found scatterplots uniquely combine high precision for both positive and negative correlations with low between-person variation, while parallel coordinates do not perform equally well across both signs [@zengReviewCollationGraphical2023; @kayWebersLawSecond2016].

**Notes:** The supporting paper emphasizes a partial ranking rather than a total ranking, so this rule is strongest as a default choice for mixed-sign use cases.

## Use when all of these are true <!-- role: context -->

- **User Goal:** Judge how strongly two quantitative variables are associated.
- **Task:** Compare or estimate correlation.
- **Data:** Two quantitative variables with correlation that may be positive, negative, or not known in advance.
- **Chart Setting:** One general-purpose chart family must serve as the default correlation view.
- **Audience:** Readers vary, and the chart should work broadly across individuals.
- **Success Criterion:** Low judgment error and stable performance across both correlation directions.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** The relationship is known to be negatively correlated and the only decision is between a scatterplot and parallel coordinates. **Why:** For negative correlation, the paper reports that scatterplots and parallel coordinates are virtually indistinguishable in performance, so the broad default advantage no longer clearly decides the choice.

## Tradeoffs of this default <!-- role: costs -->

**Sacrifice:** You give up a narrower chart choice that can be similarly strong for negative-only correlation reading.
**Risk:** Applying this as a universal total ranking can overstate small differences that the evidence only supports as grouped performance.
**Mitigation:** Use the scatterplot as the default when the sign can vary, not as proof that every non-scatter alternative is always worse.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Choosing parallel coordinates as the default because they appear slightly better in some negative-correlation cases. **Why it fails:** That treats a narrow case as a general rule and ignores that scatterplots remain high-precision across both positive and negative correlations.

## How to review the choice <!-- role: check -->

**Failure Sign:** The default correlation view switches chart family depending on sign, or parallel coordinates are kept as the default for mixed-sign use.
**Quick Check:** Render the same bivariate relation as both a scatterplot and parallel coordinates; if the design must work for either positive or negative correlation, keep the scatterplot.
**Stronger Test:** If the stated reason for parallel coordinates depends on negative-correlation performance only, verify whether the workflow ever includes positive correlations; if it does, the default should be a scatterplot.

## What to change <!-- role: fix -->

- Replace the default parallel-coordinates correlation view with a scatterplot when the chart must handle both positive and negative relationships.
- Keep the two quantitative variables on x and y position in one scatterplot specification instead of maintaining separate defaults by correlation sign.
- Remove parallel coordinates from the first-choice shortlist for mixed-sign correlation reading.
