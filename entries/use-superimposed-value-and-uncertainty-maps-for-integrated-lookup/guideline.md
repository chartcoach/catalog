---
id: use-superimposed-value-and-uncertainty-maps-for-integrated-lookup
title: Use superimposed value-and-uncertainty maps for integrated lookup
bibliography: references.bib
description: For exact lookup tasks that require combining value and uncertainty,
  use superimposed encoding on bivariate maps to improve identification accuracy and
  mitigate error-prone cross-chart matching for readers interpreting uncertainty together
  with value.
labels:
- purpose:select
- basis:empirical
- task:retrieve
- structure:single-view:use
- structure:multi-view:avoid
- quality:fidelity:use
- lever:layout-structure
- operator:uncertainty
---

## Superimpose value and uncertainty <!-- role: advice -->

Use a single superimposed map when readers must combine value and uncertainty in one judgment. For example, encode both variables in the same heatmap cell instead of asking readers to match a value heatmap to a separate uncertainty heatmap.

## Why superposition works for integrated reading <!-- role: reason -->

Superimposed maps remove a second search step. Readers can decode one location once, instead of finding the same region in two separate displays and mentally joining the results.

**Mechanism:** Superposition reduces cross-chart correspondence work when a task depends on both the value and the uncertainty of the same mark.

**Evidence:** In the paper's identification experiment, superimposed charts were significantly more accurate than juxtaposed charts for locating a target value-uncertainty pair in a heatmap-based task [@correllValueSuppressingUncertaintyPalettes2018].

## Use when value and uncertainty must be read together <!-- role: context -->

- **User Goal:** Find or verify locations that satisfy both a value condition and an uncertainty condition.
- **Task:** Integrated lookup from a bivariate legend.
- **Data:** Quantitative values paired with uncertainty for the same spatial cells or regions.
- **Chart Setting:** Dense map-like or heatmap-like displays where the same position appears in every view.
- **Audience:** Readers who need to make one decision from both variables at once.
- **Success Criterion:** Higher identification accuracy with less cross-view confusion.

## Do not use when separate pattern reading is the goal <!-- role: exceptions -->

**Break it when:** The goal is to inspect value patterns and uncertainty patterns separately rather than fuse them into one immediate judgment. **Why:** Separate views let readers consider each variable on its own, which the paper notes can be useful for orthogonal analysis even though it hurts integrated lookup.

## What you give up with superposition <!-- role: costs -->

**Sacrifice:** You lose the simplicity of two independent univariate scales.
**Risk:** Integrated color channels can be harder to decode than two separate single-variable displays.
**Mitigation:** Keep the superimposed display for fusion tasks, and add coordinated highlighting if a separate view must remain.

## Common failure in integrated uncertainty displays <!-- role: mistakes -->

**Mistake:** Put value and uncertainty in adjacent maps and expect readers to combine them quickly during lookup. **Why it fails:** Readers must perform two searches and then match the results across views, which adds error.

## Compare the two structures directly <!-- role: check -->

**Failure Sign:** Readers look back and forth between views or misidentify cells that satisfy only one of the two conditions.
**Quick Check:** Build one superimposed version and one side-by-side version of the same task, then ask a reviewer to find a specific value-uncertainty pair.
**Stronger Test:** Time and score a short A/B lookup task; keep the structure that yields fewer mismatches on integrated questions.

## Edit the layout to remove cross-view matching <!-- role: fix -->

- Merge value and uncertainty into one co-located bivariate encoding for each mark.
- Replace separate value and uncertainty heatmaps with one heatmap that encodes both variables in each cell.
- If you must keep separate views, add interaction that highlights corresponding regions across charts.
