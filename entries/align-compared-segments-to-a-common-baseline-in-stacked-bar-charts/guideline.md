---
id: align-compared-segments-to-a-common-baseline-in-stacked-bar-charts
title: Align compared segments to a common baseline in stacked bar charts
bibliography: references.bib
description: For exact comparison tasks, prefer common-baseline alignment on stacked
  bar charts to improve fidelity and mitigate length-comparison errors for viewers
  making quick visual estimates.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:bar
- quality:fidelity:use
- lever:layout-structure
- operator:difference
- reading-mode:exact
---

## Common-baseline alignment <!-- role: advice -->

Align the compared segments to a shared baseline when readers must compare heights in a stacked bar chart. For example, use an aligned stacked comparison instead of an unaligned one when viewers must judge one segment against another.

## Why a shared baseline works <!-- role: reason -->

A shared baseline turns the judgment into a more direct positional comparison. When both compared segments float inside a stack, readers must estimate lengths without a common anchor, and the surrounding stacked segments further interfere.

**Mechanism:** Common-baseline alignment reduces floating-length judgments and lowers the extra error introduced by stacked distractors.

**Evidence:** Unaligned stacked comparisons were less accurate than aligned ones, with both unalignment itself and stacked distractors contributing to the penalty; the review collates this paper as evidence on within-bar-chart comparison design [@talbotFourExperimentsPerception2014; @zengReviewCollationGraphical2023].

## When to use common-baseline alignment <!-- role: context -->

- **User Goal:** Compare two segment values exactly.
- **Task:** Estimate one segment height relative to another.
- **Data:** Quantitative segments shown within stacked bars.
- **Chart Setting:** A stacked bar chart where the comparison target is known in advance.
- **Audience:** Viewers making quick visual estimates without tools.
- **Success Criterion:** Lower comparison error between the target segments.

## When not to use common-baseline alignment <!-- role: exceptions -->

**Break it when:** The compared values are separate bars in a simple bar chart rather than segments inside a stack. **Why:** In simple bars, the main penalty came from spatial separation, not from offset segment baselines inside a stack.

## Tradeoffs of common-baseline alignment <!-- role: costs -->

**Sacrifice:** Floating stacked arrangements that leave the compared segments offset.\
**Risk:** If you keep the comparison unaligned, extra stacked segments make the judgment even harder.\
**Mitigation:** When stacking is required, prioritize baseline alignment for the comparison target.

## Common alignment mistake <!-- role: mistakes -->

**Mistake:** Asking readers to compare two floating stacked segments without a shared baseline. **Why it fails:** Unalignment and stacked distractors both increase error.

## Check baseline alignment <!-- role: check -->

**Failure Sign:** Readers misjudge which segment is closer to half or two-thirds of the other.\
**Quick Check:** Redraw the same comparison with a shared baseline and inspect whether the target ratio reads more directly.\
**Stronger Test:** Run an A/B estimate task on aligned versus unaligned versions and compare absolute error.

## Fix unaligned stacked comparisons <!-- role: fix -->

- Restructure the stack so the compared segments share a baseline.
- Avoid floating both compared segments when an exact comparison is important.
- Remove extra stacked segments around the target comparison when alignment cannot be achieved.
