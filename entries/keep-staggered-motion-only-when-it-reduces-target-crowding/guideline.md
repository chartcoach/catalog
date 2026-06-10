---
id: keep-staggered-motion-only-when-it-reduces-target-crowding
title: Keep staggered motion only when it reduces target crowding
bibliography: references.bib
description: For visual tracking during ordered-time transitions, use target-crowding
  reduction as the decision rule for staggered motion on dense dot-based views to
  improve fidelity and mitigate ineffective pacing changes for analysts.
labels:
- purpose:refine
- basis:empirical
- task:relate
- time:ordered-time
- quality:fidelity:use
- lever:interaction-access
- density:dense
- temporal-pattern:dynamic
---

## Crowding-based staggering <!-- role: advice -->

Evaluate staggered motion by whether it lowers crowding around the points users need to follow. For example, compare a direct point-cloud transition with a candidate ordering or dwell setting and keep the staggered version only when nearest-neighbor crowding drops without higher inner crowding or deformation.

## Why crowding is the right test <!-- role: reason -->

Among the measured difficulty factors, target crowding was the one most clearly linked to tracking performance and the one most likely to improve under staggering. But those improvements were uncommon and usually modest, so staggering needs a measurable crowding win to justify its extra pacing complexity.

**Mechanism:** Lower target crowding reduces close approaches and crossings between targets and distractors, which lowers the chance that viewers swap or lose the points they are following.

**Evidence:** The paper validated target crowding as a strong predictor of tracking difficulty and found that, of the tested complexity metrics, target crowding was the one that benefited most from staggering; it therefore recommends primarily considering this factor when designing staggered animations [@chevalierNotsoStaggeringEffectStaggered2014].

**Notes:** The paper found little benefit from staggering on inner crowding and found that staggering often increased deformation.

## Use when staggering is being considered <!-- role: context -->

- **User Goal:** Improve point-to-point correspondence during an animated transition.
- **Task:** Track specific points through motion while ignoring distractors.
- **Data:** Dense sets of visually similar moving dots.
- **Chart Setting:** A short point-layout transition where you are deciding whether to add staggered starts.
- **Audience:** Analysts relying on accurate visual tracking.
- **Success Criterion:** Lower tracking error than the direct animation baseline.

## When not to keep staggering <!-- role: exceptions -->

**Break it when:** The staggered version lowers crowding only by increasing inner crowding or deformation. **Why:** Those added costs can erase or reverse the crowding benefit.

## What you trade away <!-- role: costs -->

**Sacrifice:** You spend extra design effort evaluating motion order and dwell instead of assuming any staggered pacing will help.
**Risk:** A crowding improvement can still come with less predictable motion and faster individual movements.
**Mitigation:** Keep a direct animation baseline and prefer it unless the staggered version shows a clear crowding advantage without offsetting costs.

## Common crowding mistake <!-- role: mistakes -->

**Mistake:** Keeping a staggered transition because it looks less overwhelming without checking whether it actually reduces target crowding. **Why it fails:** Many staggered transitions changed crowding only modestly or worsened other difficulty factors.

## How to test the crowding benefit <!-- role: check -->

**Failure Sign:** Points still pass very close to tracked marks after staggering is added.
**Quick Check:** Compare nearest-neighbor crowding over time in the direct and staggered versions for the points a viewer is likely to follow.
**Stronger Test:** Discard staggered variants where inner crowding or deformation increases, even if target crowding drops.

## What to change <!-- role: fix -->

- Compare candidate staggering orders against a direct baseline using the crowding metric.
- Remove staggering when the measured crowding reduction is small or inconsistent.
- Reject staggered variants that improve crowding but increase deformation or inner crowding.
