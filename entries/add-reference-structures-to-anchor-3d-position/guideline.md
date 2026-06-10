---
id: add-reference-structures-to-anchor-3d-position
title: Add reference structures when 3D position is hard to decode
bibliography: references.bib
description: For lookup and compare tasks in 3D scenes with ambiguous depth, use regular
  reference structures on the display to improve fidelity and address misread spatial
  position for viewers locating marks in depth.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- quality:fidelity
- lever:layout-structure
- channel:position:use
- reading-mode:lookup
---

## Reference grids and projection cues <!-- role: advice -->

Add explicit reference structures when the depth of 3D marks is not obvious from the data alone. For example, show regular mesh lines on a surface or add projection lines, shadows, or a reference plane for points so readers can place marks in 3D space.

## Why anchoring cues matter <!-- role: reason -->

Depth is much easier to decode when the scene provides stable cues about where marks sit relative to a known structure. The paper repeatedly points to grids, reference lines, shadows, and other depth cues as the elements that make 3D position readable rather than guesswork.

**Mechanism:** Regular reference structures convert ambiguous depth into a guided spatial read, helping readers judge relative location instead of inferring it from a bare perspective view.

**Evidence:** The paper states that regular rectangular meshes provide strong perspective cues, and later notes that non-anchored 3D points are hard to locate without cues such as stereoscopic viewing, shadows, reference lines, motion parallax, lighting, or reference planes [@brath3DInfoVisHere2014].

## Use when depth is not self-evident <!-- role: context -->

- **User Goal:** Locate points or surface features accurately in 3D.
- **Task:** Read position or compare relative depth from a single view.
- **Data:** 3D points, bars, meshes, or surfaces whose position is not fully determined by obvious regular structure.
- **Chart Setting:** A 3D display that may be viewed statically or with limited interaction.
- **Audience:** Readers who need spatial decoding help from the scene itself.
- **Success Criterion:** A viewer can place marks in depth without guessing.

## When this breaks <!-- role: exceptions -->

**Break it when:** The data already supplies strong positional cues through its own regular structure, such as regularly advancing time with constrained change between intervals. **Why:** The paper notes that some structured datasets remain readable without extra cues because the data itself reveals the spatial relationships.

## What you trade away <!-- role: costs -->

**Sacrifice:** You give up some visual minimalism.
**Risk:** Too many auxiliary lines can clutter the scene.
**Mitigation:** Use regular structures that directly support spatial decoding rather than decorative 3D effects.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Show random-looking 3D points with no reference grid, reference plane, or projection cue. **Why it fails:** Viewers cannot reliably determine the points' depth from a bare static perspective.

## How to check it <!-- role: check -->

**Failure Sign:** Reviewers disagree about whether a point is in front of, behind, or aligned with another mark.
**Quick Check:** Freeze the scene and ask whether a viewer can estimate a mark's location in depth without rotating it.
**Stronger Test:** Compare the same scene with and without grid or projection cues and check whether positional judgments become stable.

## What to change <!-- role: fix -->

- Turn on mesh lines or grid lines at regular intervals.
- Add projection lines, shadows, or a visible reference plane for points.
- Remove purely decorative 3D effects that do not help readers place marks in depth.
