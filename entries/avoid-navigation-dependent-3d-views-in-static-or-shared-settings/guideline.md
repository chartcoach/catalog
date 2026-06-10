---
id: avoid-navigation-dependent-3d-views-in-static-or-shared-settings
title: Do not make 3D navigation necessary when the view must stand on its own
bibliography: references.bib
description: For presentation and review contexts with static frames or shared control,
  avoid navigation-dependent 3D views to prevent comprehension failure and address
  interaction bottlenecks for viewers who cannot steer the scene.
labels:
- purpose:refine
- basis:empirical
- quality:readability
- lever:interaction-access
- communication:workflow
---

## Static-comprehensible 3D views <!-- role: advice -->

Design the 3D scene so the key relationships remain readable without navigation when not every viewer can control the view. For example, avoid 3D scatterplots or other scenes that only become comprehensible after rotation in published images, static slides, or collaborative sessions with one controller.

## Why navigation dependence is risky <!-- role: reason -->

A 3D view fails quickly when readers must rotate it to understand it but cannot do so in the actual setting. The paper treats navigation as a critical failure point whenever the scene requires interaction to become comprehensible.

**Mechanism:** A navigation-independent view preserves the core message across screenshots, slides, and shared-control settings instead of tying understanding to one person's interaction.

**Evidence:** The paper identifies navigation as a critical problem when comprehension depends on interaction and names published images, static snapshots, PowerPoint slides, and collaborative settings with a single controller as situations where that dependency becomes a liability [@brath3DInfoVisHere2014].

## Use when the scene may be consumed without control <!-- role: context -->

- **User Goal:** Communicate or review the visualization in a setting where not everyone can interact.
- **Task:** Preserve comprehension in static or shared-control use.
- **Data:** Any 3D information display whose structure could otherwise depend on viewpoint changes.
- **Chart Setting:** Print, static export, slides, or collaborative analysis with one active controller.
- **Audience:** Viewers who may only see a fixed frame or may not control the interaction.
- **Success Criterion:** The main relationships remain understandable from the displayed view alone.

## When this breaks <!-- role: exceptions -->

**Break it when:** Every intended viewer has direct interactive control and the scene does not rely on a single privileged viewpoint. **Why:** The paper frames the problem as one of missing or restricted interaction.

## What you trade away <!-- role: costs -->

**Sacrifice:** You may show a less exploratory view than a fully navigable 3D scene could offer.
**Risk:** If applied blindly, you can simplify away useful depth relationships.
**Mitigation:** Keep the 3D context, but make sure the chosen view is interpretable before any rotation.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Assume the viewer will always rotate the scene to decode it. **Why it fails:** Static and shared-control settings remove that option and leave the view unreadable.

## How to check it <!-- role: check -->

**Failure Sign:** A screenshot of the view is confusing until someone rotates or reorients it.
**Quick Check:** Review the visualization as a single static frame and see whether the main pattern can be explained without interaction.
**Stronger Test:** Show the fixed view to someone without control and ask them to describe the main structure.

## What to change <!-- role: fix -->

- Choose a viewpoint that already exposes the main structure.
- Replace a navigation-dependent free-point view with a more anchored or regularly structured 3D arrangement.
- Add a linked 2D detail or slice view if exact reading would otherwise require navigation.
