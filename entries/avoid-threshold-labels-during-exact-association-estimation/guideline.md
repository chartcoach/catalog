---
id: avoid-threshold-labels-during-exact-association-estimation
title: Avoid threshold labels during exact numeric association estimation
bibliography: references.bib
description: For exact association estimation from scatterplots, avoid threshold labels
  in on-screen instructions to prevent anchoring and mitigate repeated guesses at
  category cutoffs for viewers entering numeric judgments.
labels:
- purpose:refine
- basis:empirical
- task:relate
- chart:scatter
- quality:fidelity
- lever:text-annotation
- reading-mode:exact
- component:label:avoid
---

## Remove threshold numbers from estimation text <!-- role: advice -->

Remove threshold numbers from on-screen instructions when viewers must enter an exact association value. For example, do not describe a scatterplot as low below 50, medium from 50 to 80, and high above 80 on the same screen where the viewer must enter a 0 to 100 estimate.

## Why threshold text anchors estimates <!-- role: reason -->

Named cutoff values become ready-made candidate answers. Readers can reuse those numbers instead of reading only from the plot.

**Mechanism:** Threshold labels prime specific values and anchor estimates at those values. This makes the entered number reflect the instruction text as well as the chart.

**Evidence:** In the linear-association task, the paper observed accuracy changes specifically at 50 and 80, the same values used in the question text to define low, medium, and high association. The authors attribute those changes to anchoring from the instructional thresholds and state that such signals should be removed in future experiments [@hullmanImpactSocialInformation2011].

**Notes:** The issue appears when the task asks for an exact numeric readout, not just a coarse category.

## Use when the screen mixes exact input with verbal categories <!-- role: context -->

- **User Goal:** Estimate a continuous value from a scatterplot.
- **Task:** Enter an exact linear-association judgment.
- **Data:** A scatterplot with a visible positive linear relationship.
- **Chart Setting:** The same screen includes instructional text or labels with numeric category cutoffs.
- **Audience:** Viewers enter a number on a 0 to 100 scale.
- **Success Criterion:** Estimates reflect the plotted pattern rather than the named thresholds.

## Do not use when the task is categorical by design <!-- role: exceptions -->

**Break it when:** The intended output is a category such as low, medium, or high rather than an exact number. **Why:** In that case the threshold labels define the task instead of acting as an unwanted anchor.

## Tradeoffs of removing the thresholds <!-- role: costs -->

**Sacrifice:** You lose a quick verbal scaffold for interpreting the scale.
**Risk:** Some viewers may feel less certain about how the numeric scale maps to broad verbal categories.
**Mitigation:** Put category explanations in practice or qualification material instead of the exact-estimation screen.

## Common failure mode: mixing category cutoffs with exact entry <!-- role: mistakes -->

**Mistake:** Keeping category labels and exact numeric input on the same screen. **Why it fails:** The category cutoffs become salient answer choices and can pull estimates toward those exact numbers.

## How to test for anchoring at the cutoffs <!-- role: check -->

**Failure Sign:** Responses spike at the same numbers used in the instructional cutoffs.
**Quick Check:** Count answers at the cutoff values and compare them with nearby values.
**Stronger Test:** Run the same estimation task with and without the threshold text and compare whether the cutoff values attract extra responses.

## What to change <!-- role: fix -->

- Delete numeric category cutoffs from the screen used for exact estimation.
- Move category explanations to a separate practice or qualification step.
- Keep only the exact numeric response scale visible while the viewer is entering the estimate.
