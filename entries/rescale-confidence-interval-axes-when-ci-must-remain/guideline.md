---
id: rescale-confidence-interval-axes-when-ci-must-remain
title: Rescale the axis when you must keep confidence intervals
bibliography: references.bib
description: For treatment-effect judgments from confidence-interval summaries, use
  axis rescaling on mean-with-interval charts to improve fidelity and mitigate exaggerated
  effect-size perception for lay readers.
labels:
- purpose:refine
- basis:empirical
- task:compare
- quality:fidelity:use
- lever:scale-order
- component:axis:use
- operator:uncertainty
- audience:general-public
---

## Rescale the axis around the broader outcome range <!-- role: advice -->

Broaden the axis when a confidence-interval plot must remain and readers will judge effect size from it. For example, keep the 95% confidence-interval bars but rescale the axis to the same range and tick pattern that would accommodate the corresponding 95% prediction intervals.

## Why axis rescaling helps <!-- role: reason -->

A tight axis around narrow confidence intervals amplifies small differences in means. Expanding the axis adds some visual context about how small those mean differences are relative to the broader spread of outcomes, so readers overstate treatment effectiveness less.

**Mechanism:** Rescaling reduces the visual exaggeration created by narrow confidence-interval bars on a tight axis, which makes effect-size judgments less extreme.

**Evidence:** In the second experiment, confidence-interval plots on rescaled axes produced more accurate willingness-to-pay, probability-of-superiority, and variability judgments than conventional confidence-interval plots, though they still performed worse than prediction intervals and animated samples [@hofmanHowVisualizingInferential2020].

**Notes:** This is a partial repair, not a full substitute for showing outcome uncertainty directly.

## Use when all of these are true <!-- role: context -->

- **User Goal:** Help readers compare treatment effectiveness from a confidence-interval chart.
- **Task:** Estimate effect size or probability of superiority from two summarized conditions.
- **Chart Setting:** The plot must retain confidence-interval bars.
- **Component:** The axis range and tick placement can still be edited.
- **Audience:** Lay readers or other nonexpert consumers of the result.
- **Success Criterion:** Judgments are less inflated than with a tightly cropped confidence-interval axis.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** You can change the uncertainty encoding itself and high-fidelity treatment-effect judgments are the priority. **Why:** Rescaled confidence intervals improved answers only somewhat, while prediction intervals and animated samples were closer to the normatively correct answers.

## Tradeoffs of axis rescaling <!-- role: costs -->

**Sacrifice:** You lose some ease in reading very small differences in means.
**Risk:** A broader axis can make mean separation harder to inspect at a glance.
**Mitigation:** Use rescaling as a fallback when confidence intervals must stay, not as the preferred format for individual-outcome judgments.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep a tight axis that hugs the confidence-interval bars. **Why it fails:** The compressed scale makes a small difference in means look disproportionately large.

## Review before publishing <!-- role: check -->

**Failure Sign:** The axis range appears to be set by the confidence-interval height rather than by plausible outcome spread.
**Quick Check:** Compare the confidence-interval plot against a version scaled to the broader prediction-interval range; if the tight-axis version makes the means look dramatically farther apart, rescale.
**Stronger Test:** Match the rescaled axis range and tick placement to the broader outcome-uncertainty range before finalizing the chart.

## Revise the chart <!-- role: fix -->

- Extend the axis to accommodate the broader 95% prediction-interval range.
- Keep the confidence-interval bars but place them on this broader axis.
- Match the tick placement and range to the broader uncertainty scale rather than to the narrow confidence intervals.
- If the chart can change format, replace the confidence-interval display with an outcome-uncertainty display instead of relying on rescaling alone.
