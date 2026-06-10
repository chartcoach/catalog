---
id: preserve-relative-geometry-when-tracking-point-identities
title: Preserve relative geometry when viewers must track point identities
bibliography: references.bib
description: For identity-preserving visual tracking during ordered-time transitions,
  avoid animation pacing that deforms relative point geometry on dot-based views to
  improve fidelity and mitigate identity swaps for analysts.
labels:
- purpose:refine
- basis:empirical
- task:relate
- time:ordered-time
- quality:fidelity:use
- lever:interaction-access
- temporal-pattern:dynamic
---

## Stable relative geometry <!-- role: advice -->

Keep the relative distances among tracked points as stable as the transition allows when viewers must know which point is which. For example, let a small set of points translate or rotate together in a direct animation instead of staggering them so the triangle they form collapses or changes shape.

## Why stable geometry helps identity tracking <!-- role: reason -->

Identity tracking depends on maintaining both where a point goes and which point it is. When the spacing among tracked points changes sharply over time, viewers are more likely to confuse their identities even if they still know the general area where the group ended up.

**Mechanism:** Stable relative geometry lets viewers preserve a coherent spatial structure for the tracked set, which reduces identity swaps among similar moving points.

**Evidence:** The paper validated deformation as a difficulty factor and found that deformation seriously impaired target identity tracking; participants were more likely to mix up identities when the shape formed by the targets distorted rather than mainly translating or rotating [@chevalierNotsoStaggeringEffectStaggered2014].

**Notes:** The effect of deformation was much smaller when viewers only needed to recover the final target set without preserving individual identities.

## Use when identity must be preserved <!-- role: context -->

- **User Goal:** Maintain which individual point is which across a transition.
- **Task:** Assign the original identities of multiple targets after the motion ends.
- **Data:** Visually identical moving points whose identities are distinguished only before the animation starts.
- **Chart Setting:** A short animated transition between two point layouts.
- **Audience:** Analysts who need identity-level correspondence, not just group-level correspondence.
- **Success Criterion:** Correct identity assignment for the tracked points.

## When not to enforce this rule <!-- role: exceptions -->

**Break it when:** Viewers only need the final group of target points and do not need to preserve which target is which. **Why:** Deformation was much less harmful in the no-identity tracking condition.

## What you trade away <!-- role: costs -->

**Sacrifice:** You give up some freedom to sequence points independently.
**Risk:** Preserving geometry can leave more crowding in some transitions.
**Mitigation:** If you relax geometry to reduce crowding, verify that identity-tracking accuracy actually improves.

## Common geometry mistake <!-- role: mistakes -->

**Mistake:** Using staggered pacing that breaks a coherent group motion into a collapsing or sharply stretching shape. **Why it fails:** Viewers are more likely to confuse the identities of the moving points.

## How to test geometry stability <!-- role: check -->

**Failure Sign:** The relative distances among tracked points change sharply, or a simple shape formed by them collapses during the animation.
**Quick Check:** Connect three sample tracked points mentally and watch whether the shape mostly translates or rotates versus strongly stretching or crossing.
**Stronger Test:** Run an identity-tracking trial where viewers must assign the original labels to the final points.

## What to change <!-- role: fix -->

- Remove staggered delays for identity-critical points and let them move together.
- Use a direct animation that keeps the tracked points moving as a coherent structure.
- Reject candidate animations that sharply increase deformation, even if they look less crowded.
