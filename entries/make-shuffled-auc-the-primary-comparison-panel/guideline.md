---
id: make-shuffled-auc-the-primary-comparison-panel
title: Make shuffled AUC the primary comparison panel
bibliography: references.bib
description: For grouped-result comparisons of fixation-prediction models, use shuffled-AUC-first
  layout on multi-view benchmark panels to improve fidelity and mitigate center-bias
  and border-driven misreading for analysts.
labels:
- purpose:refine
- basis:empirical
- scope:grouped-result
- structure:multi-view
- quality:fidelity:use
- lever:layout-structure
- communication:credibility
---

## Score-panel priority <!-- role: advice -->

Make the shuffled-AUC panel the primary readout when showing fixation-prediction model rankings. For example, rank models by shuffled AUC, place CC and NSS in secondary panels, and treat a strong centered-Gaussian score under CC or NSS as evidence of center bias rather than model quality.

## Why shuffled AUC should lead <!-- role: reason -->

Center-biased fixation datasets can make a weak center-seeking method look strong under some scores. A primary shuffled-AUC view keeps attention on off-center fixations that are harder and more informative to predict.

**Mechanism:** Shuffled AUC discounts center bias by using fixations from other images as negatives, so the headline ranking is less driven by central fixation density and border artifacts.

**Evidence:** The paper reports that CC and NSS are sensitive to center preference, that shuffled AUC tackles center bias and border effects, and that shuffled AUC is the best option for saliency-model comparison on fixation datasets [@borjiQuantitativeAnalysisHumanModel2013].

**Notes:** The paper still reports CC and NSS, but not as the preferred basis for judging model quality.

## Use when fixation benchmarks are center-biased <!-- role: context -->

- **User Goal:** Fairly compare fixation-prediction methods.
- **Task:** Rank models on natural image or video eye-tracking benchmarks.
- **Data:** Human fixation datasets with strong center clustering.
- **Chart Setting:** Multi-panel benchmark figures or leaderboards with several evaluation scores.
- **Audience:** Analysts and reviewers comparing model quality.
- **Success Criterion:** The headline ranking reflects non-trivial fixation prediction rather than dataset bias.

## Do not use it as the primary readout for single-target search arrays <!-- role: exceptions -->

**Break it when:** The comparison is limited to synthetic search patterns with one tagged target location and the goal is pure target detection. **Why:** The paper uses NSS there because a single target location makes target-hit strength the relevant score.

## What this costs <!-- role: costs -->

**Sacrifice:** The primary panel becomes less comparable to older results that emphasized CC or NSS.
**Risk:** Readers may ignore secondary score panels they already know.
**Mitigation:** Keep CC and NSS visible as secondary panels, but make the ranking and takeaway come from shuffled AUC.

## Common score-panel failure <!-- role: mistakes -->

**Mistake:** Use CC or NSS as the headline ranking on center-biased fixation datasets. **Why it fails:** A centered baseline can score well there, so the chart overstates true fixation-prediction quality.

## How to test the panel order <!-- role: check -->

**Failure Sign:** A centered-Gaussian baseline sits near the top of the headline ranking.
**Quick Check:** Re-rank the same models by shuffled AUC and see whether the order changes materially.
**Stronger Test:** Compare the headline conclusion from CC or NSS against shuffled AUC; if the main winners change, the score order is hiding center-bias effects.

## What to change <!-- role: fix -->

- Promote the shuffled-AUC ranking to the top or leftmost panel.
- Move CC and NSS into secondary panels in the same figure.
- Reword the main takeaway to cite shuffled AUC first.
- If CC or NSS stay prominent, add an explicit centered-Gaussian baseline to show how much center bias they reward.
