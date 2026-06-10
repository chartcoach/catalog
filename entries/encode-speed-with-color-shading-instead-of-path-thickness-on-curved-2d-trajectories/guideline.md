---
id: encode-speed-with-color-shading-instead-of-path-thickness-on-curved-2d-trajectories
title: Encode speed with color shading instead of path thickness on curved 2D trajectories
bibliography: references.bib
description: For speed-extremum lookup on ordered-time trajectories, prefer color
  shading for speed on curved 2D path views to improve fidelity and mitigate curvature-driven
  misreading from path thickness for readers locating fastest or slowest points.
labels:
- purpose:refine
- basis:empirical
- task:extreme
- time:ordered-time
- quality:fidelity:use
- lever:encoding
- channel:color-saturation:use
- channel:area:avoid
---

## Color for speed on curved paths <!-- role: advice -->

Encode speed with color shading when readers must find the fastest or slowest point on a curved 2D trajectory. For example, use a sequential color ramp along the path instead of widening the path to show higher speed.

## Why color beats width on curved paths <!-- role: reason -->

Color variation survives curvature better than path thickness. When the path bends, width changes become harder to judge consistently, but a sequential color ramp stays readable along the curve.

**Mechanism:** A color ramp lets readers scan for local speed changes without compensating for the visual distortion that curvature introduces into path thickness.

**Evidence:** In the speed-extremum task on curved 2D+time trajectories, color-based speed encoding ranked highest, size-based speed encoding ranked lower, and the paper recommends value-based speed encoding while discouraging size for curved paths [@perinAssessingGraphicalPerception2018; @zengReviewCollationGraphical2023].

**Notes:** The paper reports a stronger advantage for color over size on curved paths than on straight paths.

## Use when readers must locate speed extrema on a curved path <!-- role: context -->

- **User Goal:** Find where the path is fastest or slowest.
- **Task:** Identify a speed extremum at a point on the path.
- **Data:** Speed varies over ordered time on a 2D trajectory.
- **Chart Setting:** A static smoothly curved path with no sharp angles, loops, or crossings.
- **Audience:** Readers making quick chart-reading judgments.
- **Success Criterion:** More accurate identification of the fastest or slowest point.

## Do not use when color is unavailable or the path is not the tested case <!-- role: exceptions -->

- **Break it when:** The trajectory is straight-only and speed is the only important quantity. **Why:** The study found direct speed encodings to be adequate for straight paths.
- **Break it when:** The color channel is already committed elsewhere in the same view. **Why:** The source recommends segment length as the fallback when value-based speed encoding cannot be used.

## Costs of speed-by-color <!-- role: costs -->

**Sacrifice:** You spend the color channel on speed.
**Risk:** The speed ramp can conflict with other color use in the surrounding view.
**Mitigation:** If color is unavailable, move speed reading to segment spacing rather than back to path thickness on a curved path.

## Common failure mode: speed by path thickness on curves <!-- role: mistakes -->

**Mistake:** Encode speed with path thickness on a curved trajectory. **Why it fails:** Curvature distorts width judgments, and the size-based speed encoding produced lower accuracy than the color-based speed encoding.

## Review check for speed encoding <!-- role: check -->

**Failure Sign:** Reviewers disagree about where the fastest or slowest point falls on the curved path.
**Quick Check:** Render the same curved trajectory once with speed-by-color and once with speed-by-thickness, then ask a reviewer to mark the fastest or slowest point in both versions.
**Stronger Test:** Repeat that A/B comparison on several simple curved trajectories and keep the color version if it is more accurate across the set.

## Fix the speed encoding <!-- role: fix -->

- Replace speed-varying path thickness with a sequential speed color ramp.
- Keep path width constant once color carries speed on the curved trajectory.
- If color is unavailable, add equal-time ticks so segment spacing, not path width, carries speed.
