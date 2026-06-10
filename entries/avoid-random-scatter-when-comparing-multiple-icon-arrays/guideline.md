---
id: avoid-random-scatter-when-comparing-multiple-icon-arrays
title: Avoid random scatter when comparing multiple icon arrays
bibliography: references.bib
description: For first-glance comparison of multiple proportions under brief viewing,
  avoid random arrangement on icon-array graphics to improve fidelity and address
  rank confusion between moderately different values for public audiences.
labels:
- purpose:refine
- basis:empirical
- task:compare
- structure:multi-view
- operator:difference
- reading-mode:overview
- lever:layout-structure
- quality:fidelity
---

## Sequential arrangement for comparison <!-- role: advice -->

Use a sequential block arrangement when readers must compare two or more icon arrays at a glance. For example, line up the highlighted figures in each array instead of scattering them randomly when showing before-and-after risks or two risks that differ by about 10 percentage points.

## Why random scatter hurts comparison <!-- role: reason -->

Comparison works better when each proportion appears as one contiguous mass. Random scatter obscures moderate differences, so viewers can reverse the ordering of two values that are actually distinct.

**Mechanism:** Sequential blocks let viewers compare adjacent areas directly, while random layouts add visual noise and force mental aggregation before the comparison can happen.

**Evidence:** More than one quarter of respondents confused random icon arrays showing 29% versus 40%, while far fewer made that error with sequential arrays; random arrangements also produced higher first-glance estimates than sequential ones for most tested proportions [@anckerEffectArrangementStick2011].

**Notes:** The paper states that small to moderate differences might become detectable after a longer examination period.

## Where to use sequential comparison layouts <!-- role: context -->

- **User Goal:** Help viewers see which of two or more proportions is larger.
- **Task:** Rank values or judge a moderate difference quickly.
- **Data:** Multiple part-whole proportions shown in separate icon arrays.
- **Chart Setting:** Arrays are compared in one session, likely at first glance, without relying on counting.
- **Audience:** Consumers or patients reading risk graphics.
- **Success Criterion:** Readers correctly order the arrays and notice moderate differences immediately.

## When this rule can be relaxed <!-- role: exceptions -->

**Break it when:** Viewers can inspect the graphic for longer and immediate discriminability is not required. **Why:** The paper notes that small to moderate differences may become detectable after a longer examination period.

## Tradeoffs of sequential comparison layouts <!-- role: costs -->

**Sacrifice:** The arrays lose the scattered appearance of random placement.
**Risk:** Sequential layout improves comparison but does not make the values exact; large blocked proportions were still overestimated.
**Mitigation:** Do not rely on first-glance comparison alone when the exact percentage difference is important.

## Common comparison mistake <!-- role: mistakes -->

**Mistake:** Use random scatter in every array and assume the difference will still be obvious because the counts differ. **Why it fails:** Moderate differences can be hard to see and may even be ranked in the wrong order.

## How to check the comparison view <!-- role: check -->

**Failure Sign:** Viewers reverse the order of two arrays with a known moderate difference.
**Quick Check:** Show the pair for about 10 seconds and ask which one is larger.
**Stronger Test:** Compare a random version and a sequential-block version of the same pair, and keep the version with fewer rank reversals.

## What to change <!-- role: fix -->

- Replace the random scatter in each array with a contiguous block of the same size.
- Keep the grid size and highlighted count constant across the compared arrays while changing only the arrangement.
- Re-test whether viewers can rank the arrays correctly at first glance.
