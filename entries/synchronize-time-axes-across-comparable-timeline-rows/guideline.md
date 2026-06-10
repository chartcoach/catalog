---
id: synchronize-time-axes-across-comparable-timeline-rows
title: Synchronize time axes across comparable timeline rows
bibliography: references.bib
description: For cross-row comparison of predictive uncertainty in multi-row timeline
  views, use a shared axis across rows to improve fidelity and mitigate misleading
  similarity between differently scaled predictions for quick mobile comparison.
labels:
- purpose:refine
- basis:empirical
- task:compare
- structure:small-multiples
- chart:timeline
- quality:fidelity:use
- lever:layout-structure
- component:axis:use
---

## Shared row axes <!-- role: advice -->

Use one synchronized time axis across comparable rows when users need to compare predicted timing or uncertainty between items. For example, keep each timeline row on the same minute scale instead of giving each row its own fitted range, so narrow and wide predictive spreads remain visually distinguishable across rows.

## Why shared row axes work <!-- role: reason -->

Cross-row comparison depends on a stable positional reference. If each row rescales itself to its own range, different predictions can take on similar shapes and widths even when their timing uncertainty differs substantially.

**Mechanism:** A shared axis preserves the meaning of horizontal position and spread across rows. This prevents per-row scaling from flattening meaningful differences in variance.

**Evidence:** In the design process, row-specific relative timelines were rejected because they were very difficult to compare across rows; different-variance predictions could look similar once each row's timeline and density were rescaled independently [@kayWhenIshMy2016].

## When to use shared row axes <!-- role: context -->

- **User Goal:** Compare several upcoming options at once.
- **Task:** Compare arrival times, spread, or relative certainty across rows.
- **Data:** Multiple predictive distributions with different variances.
- **Chart Setting:** Multi-row mobile timeline displays with one row per predicted item or route.
- **Audience:** Everyday users scanning several rows quickly.
- **Success Criterion:** Row-to-row comparisons of timing and uncertainty remain trustworthy.

## When not to use shared row axes <!-- role: exceptions -->

**Break it when:** Users inspect one prediction at a time and do not need row-to-row comparison. **Why:** The main problem with per-row scaling is that it breaks comparison across rows.

## Tradeoffs of shared row axes <!-- role: costs -->

**Sacrifice:** You lose some local zoom on individual rows.
**Risk:** Low-variance predictions may occupy less of the available row space and reveal less local detail.
**Mitigation:** Accept some lost local detail to preserve comparability across the full set of rows.

## Common mistakes with shared row axes <!-- role: mistakes -->

**Mistake:** Giving each row its own time range so every prediction fills its row. **Why it fails:** Rescaling can make very different uncertainty ranges look similar.

## How to check shared row axes <!-- role: check -->

**Failure Sign:** Two rows with different numeric ranges look similarly wide after scaling.
**Quick Check:** Put a narrow and a wide prediction on adjacent rows; if viewers struggle to say which is more variable, the axes are not comparable enough.
**Stronger Test:** Compare a shared-axis mockup against a per-row-axis mockup and keep the version where users correctly compare spread across rows.

## How to fix shared row axes <!-- role: fix -->

- Lock all comparable rows to one shared time scale.
- Remove per-row auto-scaling that resizes each distribution to its own local range.
- If space is tight, reduce local detail rather than changing the row scale from one row to the next.
