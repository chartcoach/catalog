---
id: pair-3d-overview-with-linked-2d-detail
title: Pair a 3D overview with linked 2D detail views for precise reading
bibliography: references.bib
description: For compare tasks on complex 3D data spaces, use a multi-view layout
  with a 3D overview and linked 2D slices to improve fidelity and address imprecise
  direct reading from a 3D-only single view for readers who need both context and
  exact values.
labels:
- purpose:select
- basis:empirical
- task:compare
- structure:multi-view:use
- structure:single-view:avoid
- quality:fidelity
- lever:layout-structure
- reading-mode:exact
---

## 3D context plus 2D focus <!-- role: advice -->

Use a linked 3D overview plus 2D detail view instead of a 3D-only single view when readers need both the global data shape and exact readout. For example, keep the 3D surface or other 3D structure as the context and index, then show a coordinated 2D slice through the selected region for precise estimation and comparison.

## Why the paired views work <!-- role: reason -->

The 3D view helps readers understand the information space, while the 2D slice gives them a place to read exact values and comparisons more reliably. The paper presents this as a practical division of labor between overview and precision.

**Mechanism:** The overview view supports the mental model and selection of where to inspect, while the linked 2D view handles the exact reading task that 3D perspective performs less accurately.

**Evidence:** The paper states that in linked 3D-and-2D views, the 2D slices can be used for accurate estimation and comparison while the 3D view provides the global context and can act as an index into specific detailed views; it gives a deployed professional example of this pattern [@brath3DInfoVisHere2014].

## Use when one view cannot do both jobs well <!-- role: context -->

- **User Goal:** Read exact values without losing the global 3D structure.
- **Task:** Compare precise values inside a larger 3D information space.
- **Data:** A 3D representation that supports meaningful cross-sections or focused subviews.
- **Chart Setting:** Coordinated views are available, and the 3D view can indicate where the 2D detail should come from.
- **Audience:** Readers who need both exploration context and accurate readout.
- **Success Criterion:** Users can locate the relevant area in 3D and then read the selected slice precisely in 2D.

## When this breaks <!-- role: exceptions -->

**Break it when:** The 3D view cannot serve as a meaningful context or cannot act as an index to the detailed 2D view. **Why:** The paper's rationale depends on the 3D overview orienting the user and pointing to the detailed slice.

## What you trade away <!-- role: costs -->

**Sacrifice:** You use more screen space than a single view.
**Risk:** Poor coordination between the views can make the layout feel split rather than complementary.
**Mitigation:** Keep the 3D view responsible for context and selection, and keep the 2D view responsible for exact reading.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Ask readers to make exact comparisons directly from the 3D view alone. **Why it fails:** The paper treats the 2D slice as the more accurate place for estimation and comparison.

## How to check it <!-- role: check -->

**Failure Sign:** Users can see where a feature sits in the 3D space but cannot read its exact profile or compare it accurately.
**Quick Check:** Try answering a precise comparison from the 3D view alone; if the answer remains approximate, the layout needs a 2D detail.
**Stronger Test:** Compare a 3D-only view against a linked 3D-plus-2D view on the same task and see whether the latter supports more accurate readout without losing context.

## What to change <!-- role: fix -->

- Add a coordinated 2D slice or profile view next to the 3D overview.
- Make the 3D view select or indicate the specific slice shown in 2D.
- Keep the 3D view as context and index rather than the sole exact-reading surface.
