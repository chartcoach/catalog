---
id: keep-margin-of-error-and-comparison-values-on-the-chart
title: Keep margin-of-error and comparison values on the chart instead of moving them
  into text
bibliography: references.bib
description: For inferential judgments of mean and error, avoid text annotation on
  bar charts for comparison values or margins of error to prevent inaccuracy and address
  failed bias mitigation for viewers without deep statistical training.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:bar
- quality:fidelity
- lever:text-annotation
- operator:uncertainty
---

## Keep critical uncertainty values in the graphic <!-- role: advice -->

Keep the comparison value and the margin of error encoded directly in the chart instead of shifting them into text as a repair for bar-chart bias. For example, do not remove error bars and rely on a textual margin-of-error note, and do not replace a plotted comparison point with prose below the chart when viewers must judge outcomes relative to the mean.

## Why text relocation makes inference worse <!-- role: reason -->

Moving critical values into text forces readers to mentally project those values back into the plotting space. That extra projection step makes the relationship between the value, the mean, and the uncertainty harder to judge.

**Mechanism:** When viewers must imagine where a textual value falls relative to a bar and its uncertainty, accuracy drops; moving values to text does not reliably remove the bar’s containment cue and can even raise confidence while lowering correctness.

**Evidence:** In the textual one-sample experiment, moving only the compared outcome into text did not remove within-the-bar bias, and moving both the compared outcome and the margin of error into text reduced the bias only by sharply lowering accuracy while increasing confidence [@correllErrorBarsConsidered2014].

## Use when the chart must support outcome judgments <!-- role: context -->

- **User Goal:** Judge whether a possible outcome is higher or lower than the likely result, or assess how likely a specific outcome is.
- **Task:** Compare a proposed value against a mean with uncertainty.
- **Data:** A sample mean paired with a margin of error or confidence interval.
- **Chart Setting:** Bar charts where the designer is considering moving uncertainty values or comparison values into labels, legends, or text below the plot.
- **Audience:** Readers with limited statistical background.
- **Success Criterion:** Directional judgments stay accurate and confidence stays aligned with uncertainty.

## Do not use when the chart is not for inferential outcome judgments <!-- role: exceptions -->

**Break it when:** Readers do not need to compare specific outcomes against the mean or margin of error. **Why:** The observed failure came from asking readers to project textual uncertainty values into chart space for inferential tasks.

## Tradeoffs of keeping the values visual <!-- role: costs -->

**Sacrifice:** Some compactness in the surrounding text or legend.
**Risk:** If you keep the bar chart itself, restoring the values visually does not remove the underlying within-the-bar bias.
**Mitigation:** Change the visual encoding rather than relying on text relocation as the fix.

## Common partial move that still fails <!-- role: mistakes -->

**Mistake:** Move only the comparison value into text while leaving the bar and error bars intact. **Why it fails:** The bar body still acts as a containment cue, so the bias remains.

## Check whether readers must mentally project text into the plot <!-- role: check -->

**Failure Sign:** A reader has to imagine where a textual value falls relative to the bar or its uncertainty.
**Quick Check:** If the proposed outcome or the margin of error can only be interpreted by mentally mapping text back onto the y-axis, reject the change.
**Stronger Test:** Ask a few readers whether the actual outcome is likely higher or lower than the stated value; if accuracy drops while confidence rises, keep the values in the chart.

## Restore visual encoding or change the chart <!-- role: fix -->

- Put the comparison value back into the plotting area as a mark.
- Put the margin of error back into a visual uncertainty encoding instead of text alone.
- If the bar still biases judgment, replace the bar chart with a symmetric encoding such as a violin or gradient plot.
