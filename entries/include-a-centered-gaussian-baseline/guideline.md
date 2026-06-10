---
id: include-a-centered-gaussian-baseline
title: Include a centered Gaussian baseline
bibliography: references.bib
description: For grouped-result comparisons of fixation-prediction models on natural
  image or video datasets, use a centered Gaussian baseline in the benchmark to improve
  trust and mitigate mistaking dataset center bias for model quality for analysts.
labels:
- purpose:refine
- basis:empirical
- task:compare
- scope:grouped-result
- quality:trust:use
- lever:layout-structure
- communication:credibility
---

## Center-bias baseline <!-- role: advice -->

Include a centered Gaussian baseline whenever you rank fixation-prediction methods on natural scenes. For example, add a 2D Gaussian centered in the image as a benchmark row or series, compare its score against the learned models, and read unusually strong Gaussian performance under CC or NSS as a warning that the dataset is highly center-biased.

## Why the baseline should be visible <!-- role: reason -->

A trivial centered pattern can look strong when viewers mostly fixate near the middle. Showing that baseline makes it obvious when the comparison is rewarding dataset bias instead of real prediction.

**Mechanism:** The baseline gives readers a direct reference for how much of the reported performance can be explained by center preference alone.

**Evidence:** The paper introduces a centered Gaussian as a simple but powerful baseline, expects it to predict gaze well when fixations cluster at the image center, and uses its high CC and NSS scores to demonstrate strong center bias in several datasets [@borjiQuantitativeAnalysisHumanModel2013].

**Notes:** In the paper, the Gaussian baseline falls to the bottom under shuffled AUC, which helps confirm that the score discounts center bias.

## Use when the benchmark predicts gaze locations <!-- role: context -->

- **User Goal:** Judge whether model gains exceed a trivial center-focused strategy.
- **Task:** Compare fixation-prediction methods on natural images or videos.
- **Data:** Eye-tracking datasets where fixation density may cluster near the center.
- **Chart Setting:** Ranked benchmark charts, tables, or score panels.
- **Audience:** Analysts and reviewers evaluating model credibility.
- **Success Criterion:** The chart distinguishes real prediction skill from center bias.

## Do not use it for single-target search evaluation <!-- role: exceptions -->

**Break it when:** The task is synthetic odd-target detection rather than gaze prediction in natural scenes. **Why:** The Gaussian baseline is meant to expose center concentration in fixation data, not to score a single tagged target location.

## What this costs <!-- role: costs -->

**Sacrifice:** The comparison allocates one slot to a trivial reference instead of another method.
**Risk:** Readers may mistake the baseline for a competitive model rather than a diagnostic control.
**Mitigation:** Label it explicitly as a center-bias baseline.

## Common baseline failure <!-- role: mistakes -->

**Mistake:** Omit the centered baseline and interpret high CC or NSS scores as proof of strong off-center prediction. **Why it fails:** A center-seeking reference can achieve high scores on these datasets without modeling the harder fixation behavior.

## How to test whether the baseline changes the story <!-- role: check -->

**Failure Sign:** The centered Gaussian ranks near the top on the displayed score.
**Quick Check:** Add the Gaussian baseline to the current benchmark and see whether it challenges the apparent leaders.
**Stronger Test:** Compare the baseline's position under CC or NSS against its position under shuffled AUC.

## What to change <!-- role: fix -->

- Add a centered Gaussian row or series to the benchmark.
- Label it as a center-bias baseline rather than as a full model.
- Score it with the same metrics used for the other methods.
- If it ranks strongly, add or promote a shuffled-AUC panel or a low-center-bias subset panel.
