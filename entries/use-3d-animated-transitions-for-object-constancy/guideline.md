---
id: use-3d-animated-transitions-for-object-constancy
title: Use 3D animated transitions to preserve object constancy between related 2D
  views
bibliography: references.bib
description: For transitions between related 2D views of the same records, use 3D
  animated transitions to improve insight and address label-rereading and motion occlusion
  during view changes for readers tracking items across representations.
labels:
- purpose:refine
- basis:empirical
- task:relate
- quality:insight
- lever:interaction-access
- temporal-pattern:dynamic
---

## 3D transitions between related 2D views <!-- role: advice -->

Animate shared objects through a 3D intermediate state when switching between related 2D charts of the same data. For example, move between a line chart and a bar chart by lifting the marks through 3D so readers can visually track the same items instead of re-reading labels after the switch.

## Why the transition helps <!-- role: reason -->

A continuous motion path lets viewers follow the same objects as they change form and position. The paper treats 3D transitions as a way to maintain object constancy across familiar 2D representations while also revealing a mental model of how the attributes relate.

**Mechanism:** Motion shifts some of the cognitive work from label matching to visual tracking, reducing the burden of reconstructing which object in one view corresponds to which object in the next.

**Evidence:** The paper states that object constancy reduces cognitive burden by letting viewers use preattentive motion to track data through transitions, and it argues that 3D transitions between related 2D views can reduce occlusion problems seen in some 2D transitions while exposing a useful 3D mental model of attribute relationships [@brath3DInfoVisHere2014].

## Use when the same items reappear in another view <!-- role: context -->

- **User Goal:** Follow the same records across a change in chart form.
- **Task:** Relate one representation to another without losing track of identity.
- **Data:** A shared dataset that can be shown in two related 2D views.
- **Chart Setting:** An interactive display where an animated transition is available.
- **Audience:** Readers who would otherwise need to remap identity by labels alone.
- **Success Criterion:** Users can visually track objects during the switch and understand how the two views connect.

## When this breaks <!-- role: exceptions -->

**Break it when:** The medium is static or the transition cannot be shown as motion. **Why:** The benefit depends on animation and object tracking through time.

## What you trade away <!-- role: costs -->

**Sacrifice:** You add temporal complexity to a view change that could otherwise be instantaneous.
**Risk:** If the transition does not preserve identity clearly, motion becomes decoration rather than guidance.
**Mitigation:** Use the transition only between views that share stable underlying objects.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Replace one 2D view with another abruptly and expect readers to reconnect items by labels alone. **Why it fails:** The switch removes object constancy and increases the need for sequential re-reading.

## How to check it <!-- role: check -->

**Failure Sign:** Readers lose track of which object in the second view came from which object in the first.
**Quick Check:** Watch the transition and verify that a single item's path can be followed from start to finish.
**Stronger Test:** Compare the animated 3D transition against an abrupt switch and see whether readers can more easily explain the correspondence between views.

## What to change <!-- role: fix -->

- Insert a smooth animated transition instead of an abrupt chart swap.
- Route the transition through a 3D intermediate arrangement that keeps the same objects visible.
- Keep identity stable so the moving objects can be tracked visually across the full change.
