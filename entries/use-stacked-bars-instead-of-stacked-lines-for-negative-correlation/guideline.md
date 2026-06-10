---
id: use-stacked-bars-instead-of-stacked-lines-for-negative-correlation
title: Use stacked bar charts instead of stacked line charts for negative correlation
  judgments
bibliography: references.bib
description: For association judgments, prefer stacked bar charts over stacked line
  charts on negatively correlated quantitative series to improve fidelity and address
  weaker discrimination of correlation strength for people comparing opposite-moving
  values.
labels:
- purpose:select
- basis:empirical
- task:relate
- chart:bar:use
- chart:line:avoid
- quality:fidelity
- lever:chart-family
- operator:association
---

## Choose stacked bars over stacked lines for negative relationships <!-- role: advice -->

Use a stacked bar chart instead of a stacked line chart when viewers need to judge the strength of a negative correlation. For example, if two quantitative series move in opposite directions and you are choosing between these two stacked forms, use stacked bars rather than stacked lines.

## Why the stacked bar performs better here <!-- role: reason -->

Among the stacked variants, stacked bars gave the strongest negative-correlation judgments. Stacked lines were a weaker option for the same task.

**Mechanism:** The stacked bar form made differences in negative relationship strength easier to discriminate than the stacked line form, which supported less precise judgments.

**Evidence:** For negatively correlated data, stacked bar charts significantly outperformed stacked line charts in the paper's correlation-judgment experiment and Weber-model analysis [@harrisonRankingVisualizationsCorrelation2014].

**Notes:** The paper reports participant comments suggesting that viewers attended to different visual cues in stacked lines than in stacked bars.

## Use when the negative relationship is the thing being judged <!-- role: context -->

- **User Goal:** Let viewers decide which negative relationship is stronger.
- **Task:** Compare association strength between two quantitative series.
- **Data:** Two quantitative series with negative correlation.
- **Chart Setting:** A stacked presentation is desired and the choice is between stacked bars and stacked lines.
- **Success Criterion:** Viewers can more reliably distinguish stronger from weaker negative correlations.

## Do not extend this contrast to unsupported sign conditions <!-- role: exceptions -->

**Break it when:** The relationship to be judged is positive rather than negative. **Why:** Positive stacked-line and positive stacked-bar conditions frequently hit the study's chance boundary, so this contrast was not supported for positive correlations.

## Costs of changing the stacked form <!-- role: costs -->

**Sacrifice:** This rule only resolves the negative-correlation case.
**Risk:** Applying it blindly to positive correlations can claim a benefit the study did not establish.
**Mitigation:** Choose between stacked forms separately for positive and negative relationships.

## Common failure mode in this comparison <!-- role: mistakes -->

**Mistake:** Keep the stacked line chart because it appears visually similar to the stacked bar alternative. **Why it fails:** The study found that these similar-looking stacked forms did not provide the same correlation-judgment precision.

## How to test the choice <!-- role: check -->

**Failure Sign:** Viewers disagree about which negative stacked-line relationship is stronger.
**Quick Check:** Show the same negative relationship as stacked bars and as stacked lines, then ask which version makes the stronger correlation easier to see.
**Stronger Test:** Run repeated paired comparisons on both chart types and keep the one with more consistent correct choices.

## What to change <!-- role: fix -->

- Replace the stacked line chart with a stacked bar chart for the negative-correlation view.
- Compare both versions on the same negative dataset before standardizing a stacked form.
- Separate positive and negative relationship cases instead of reusing one stacked chart choice everywhere.
