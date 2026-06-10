---
id: do-not-use-caption-only-fixes-for-ci-charts
title: Do not rely on caption text alone to correct a confidence-interval chart
bibliography: references.bib
description: For treatment-effect judgments from confidence-interval summaries, avoid
  caption-only annotation on mean-with-interval charts to prevent persistent overestimation
  of treatment effectiveness and address misreading of inferential uncertainty for
  lay readers.
labels:
- purpose:refine
- basis:empirical
- task:compare
- quality:fidelity:use
- lever:text-annotation
- component:caption:avoid
- operator:uncertainty
- audience:general-public
---

## Change the chart, not just the caption <!-- role: advice -->

Change the visual encoding instead of trying to repair a confidence-interval chart with more caption text. For example, do not keep the same 95% confidence-interval bars and add extra text about prediction intervals; replace the interval encoding or rescale the axis, then make the caption match the plot.

## Why caption-only fixes fall short <!-- role: reason -->

The visual marks dominate effect-size perception in these charts. Extra explanation in the caption does not undo the effect of narrow confidence-interval bars enough to bring judgments close to those produced by outcome-uncertainty displays.

**Mechanism:** Readers anchor on the displayed intervals, so added text about other statistics does not sufficiently change how large or reliable the treatment looks.

**Evidence:** In the first experiment, adding extra caption text about additional interval information reduced the bias only somewhat; participants still judged the same confidence-interval plots as showing a more effective treatment than prediction-interval plots [@hofmanHowVisualizingInferential2020].

**Notes:** Extra text helped less than changing the plot itself.

## Use when all of these are true <!-- role: context -->

- **User Goal:** Help readers judge whether a treatment is effective.
- **Task:** Compare two summarized conditions from a plotted result.
- **Chart Setting:** The figure currently uses confidence-interval bars, and the proposed repair is to add explanatory text.
- **Component:** The caption or surrounding text can be edited.
- **Audience:** Lay readers or other nonexpert consumers of the result.
- **Success Criterion:** The revision materially changes the judgment readers form from the figure.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** The plot itself already encodes outcome uncertainty and the caption is only reinforcing what is shown. **Why:** The failed repair in the study was adding extra text while leaving a confidence-interval visualization unchanged.

## Tradeoffs of rejecting caption-only fixes <!-- role: costs -->

**Sacrifice:** You give up the convenience of a text-only revision.
**Risk:** Changing the plot may require more space or rework than editing the caption.
**Mitigation:** If confidence-interval bars must remain, change the axis as well rather than only lengthening the caption.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Add definitions or extra text about prediction intervals while leaving the confidence-interval marks unchanged. **Why it fails:** The chart still visually emphasizes inferential uncertainty, so readers continue to overestimate treatment effectiveness.

## Review before publishing <!-- role: check -->

**Failure Sign:** The proposed revision changes words but not marks.
**Quick Check:** Compare the before and after figures; if the intervals and axis are unchanged, do not expect the bias to disappear.
**Stronger Test:** Compare the caption-only revision against a plot revision such as a prediction-interval version or a rescaled confidence-interval version before publication.

## Revise the chart <!-- role: fix -->

- Replace the confidence-interval encoding with a prediction-interval encoding when readers must judge likely individual outcomes.
- If confidence intervals must stay, rescale the axis instead of only adding caption text.
- After changing the plot, rewrite the caption so it matches the displayed uncertainty.
