---
id: add-a-low-center-bias-subset-panel
title: Add a low-center-bias subset panel
bibliography: references.bib
description: For grouped-result comparisons of fixation-prediction models on center-biased
  datasets, use a low-center-bias subset panel in a multi-view benchmark to improve
  fidelity and address over-crediting center-focused models for analysts.
labels:
- purpose:refine
- basis:empirical
- task:compare
- scope:grouped-result
- structure:multi-view
- quality:fidelity:use
- lever:layout-structure
- communication:credibility
---

## Low-center-bias subset view <!-- role: advice -->

Add a separate low-center-bias subset panel when the full fixation dataset is strongly centered. For example, compute a center-bias ratio from pooled fixations, select images with CBR below the paper's threshold at the 40% radius level, and show the subset ranking beside the full-dataset ranking.

## Why the subset panel matters <!-- role: reason -->

Strong central clustering can hide which methods really predict off-center gaze. A low-center-bias subset surfaces the harder cases that are more informative for comparison.

**Mechanism:** The subset panel reduces the influence of central fixation density, so readers can judge how methods behave on off-center fixations rather than on the dataset's viewing bias.

**Evidence:** The paper introduces a center-bias ratio, uses a 40% radius criterion with a threshold of 0.7 to select less center-biased images, and shows that this second-order analysis helps differentiate model behavior on off-center fixations while the centered Gaussian performs poorly there [@borjiQuantitativeAnalysisHumanModel2013].

**Notes:** The paper reports that only a small fraction of images passed this filter in the tested still-image datasets.

## Use when the full benchmark is center-heavy <!-- role: context -->

- **User Goal:** Evaluate non-trivial fixation prediction rather than center preference.
- **Task:** Compare models on natural-scene eye-tracking datasets.
- **Data:** Pooled human fixations with strong center bias in the full dataset.
- **Chart Setting:** Multi-view benchmark figure with room for a subset result beside the full result.
- **Audience:** Analysts and reviewers checking fairness of model comparisons.
- **Success Criterion:** Off-center prediction differences become visible.

## Do not use it when no valid subset exists <!-- role: exceptions -->

**Break it when:** No images pass the center-bias filter. **Why:** The paper reports a dataset where none of the images met the threshold, so a low-center-bias subset view could not be formed.

## What this costs <!-- role: costs -->

**Sacrifice:** The subset panel uses fewer observations than the full dataset.
**Risk:** Scores may become noisier because the sample is much smaller.
**Mitigation:** Show the subset size directly in the panel so readers can judge stability.

## Common subset-panel failure <!-- role: mistakes -->

**Mistake:** Replace the full-dataset result with the low-center-bias subset. **Why it fails:** The paper uses the subset as a second view, not as a full replacement for the original benchmark.

## How to test whether the subset panel is needed <!-- role: check -->

**Failure Sign:** The full-dataset ranking stays strong for a centered baseline or mostly reflects central fixation density.
**Quick Check:** Compute the center-bias ratio at the 40% radius level and count how many images fall below 0.7.
**Stronger Test:** Compare model rankings between the full dataset and the low-center-bias subset; if the order changes, keep both views.

## What to change <!-- role: fix -->

- Pool fixations across viewers for each image without Gaussian smoothing before computing center bias.
- Compute the center-bias ratio across concentric central circles and apply the 40% radius threshold used in the paper.
- Add a separate subset panel with its own sample size.
- If no images pass the threshold, omit the subset panel rather than forcing a tiny or invalid subset.
