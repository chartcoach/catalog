---
id: separate-shape-symbols-across-sci-dimensions
title: Separate shape symbols across segmentability, compactness, and spikiness
bibliography: references.bib
description: For rapid comparison in dense shape-encoded plots, prefer shape choices
  on categorical symbol sets that differ on segmentability, compactness, and spikiness
  to improve readability and mitigate confusion between visually similar symbols for
  viewers scanning many marks at once.
labels:
- purpose:refine
- basis:empirical
- task:compare
- data:categorical
- quality:readability:use
- lever:encoding
- density:dense
- channel:shape:use
---

## Shape set separation <!-- role: advice -->

Choose category shapes that are far apart on segmentability, compactness, and spikiness. For example, in a shape-encoded scatterplot or glyph set, mix shapes with clear joints or intersections, shapes with holes or enclosed space, and smooth versus spiky contours, rather than choosing several smooth open shapes or several cross-like shapes that differ only slightly.

## Why separated shapes work <!-- role: reason -->

Shape symbols are easier to distinguish in parallel when they differ along multiple preattentive shape dimensions instead of only in small local contour details.

**Mechanism:** Spreading a symbol set across segmentability, compactness, and spikiness gives viewers more than one fast visual cue for separating groups in a dense display.

**Evidence:** Across 91 pairs of 14 shapes, discriminability in a brief masked texture-segregation task was explained very well by a three-dimensional shape space consisting of segmentability, compactness, and spikiness (r = 0.974). The paper then used that space to identify a well-separated six-shape set and showed how default scatterplot symbol sets could be improved by replacing clusters of similar shapes with shapes that are farther apart in this space [@huangSpacePreattentiveShape2020].

**Notes:** In this paper, segmentability generalizes the older idea of intersection, compactness generalizes closure and concavity, and spikiness generalizes line termination.

## Use when many marks must be told apart <!-- role: context -->

- **User Goal:** Distinguish several groups or series quickly by shape.
- **Task:** Glanceable separation of subsets without comparing symbols one by one.
- **Data:** Categories are encoded with symbol shape.
- **Chart Setting:** Many symbols appear at once in the same view, such as a dense scatterplot or glyph display.
- **Audience:** Readers must scan the display in parallel rather than inspect one mark at a time.
- **Success Criterion:** Groups are easy to tell apart at a glance.

## Do not use when shape reading is one-by-one or outside the tested symbol class <!-- role: exceptions -->

- **Break it when:** Readers mainly compare one symbol against another in isolation or inspect detailed form. **Why:** The rule comes from preattentive multi-item discrimination and the paper says it may generalize only partly to one-to-one comparison tasks.
- **Break it when:** The symbols are not 2D filled geometric shapes, such as 3D shapes, line drawings, or real-world silhouettes. **Why:** The experiment did not establish the same space for those shape classes.

## Tradeoffs of maximizing shape separation <!-- role: costs -->

**Sacrifice:** You optimize the shape encoding for fast parallel discrimination, not for detailed postattentive shape comparison.\
**Risk:** The benefit drops if added shapes fall back into the same local region of shape space.\
**Mitigation:** Add a new shape only when it introduces a new contrast in joints, enclosed space, or contour spikiness.

## Common failure mode in shape selection <!-- role: mistakes -->

**Mistake:** Choosing multiple shapes from the same local family, such as several smooth open shapes or several cross-like shapes. **Why it fails:** Shapes that do not differ much on segmentability, compactness, or spikiness are not very distinguishable in dense displays.

## Check whether the shape set is too clustered <!-- role: check -->

**Failure Sign:** Two or more groups blur together unless the viewer inspects symbols one by one.\
**Quick Check:** Inspect the set for SCI spread: does it include clear variation in joints or intersections, holes or enclosed space, and smooth versus spiky contours?\
**Stronger Test:** Put the symbols into a dense mockup and compare them against a more separated set; if the groups are not easier to separate at a glance, the current set is too clustered.

## Fix a weak shape set <!-- role: fix -->

- Replace one near-duplicate smooth open shape with a shape that has a clear joint or intersection.
- Replace one near-duplicate non-holed shape with a shape that has a hole or stronger enclosed-space contrast.
- Replace one near-duplicate smooth contour with a visibly spikier or noticeably smoother contour.
- Remove shapes that add only small local contour changes but no new SCI contrast.
