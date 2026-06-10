---
id: encode-elapsed-time-with-segment-length-ticks-on-simple-2d-trajectories
title: Encode elapsed time with segment-length ticks on simple 2D trajectories
bibliography: references.bib
description: For exact time lookup on ordered-time trajectories, prefer segment-length
  ticks on simple 2D path views to improve fidelity and mitigate misreading of elapsed
  time from color shading for readers locating time at a point on the path.
labels:
- purpose:refine
- basis:empirical
- time:ordered-time
- quality:fidelity:use
- lever:encoding
- operator:lookup
- channel:length:use
- channel:color-saturation:avoid
---

## Time ticks for elapsed time <!-- role: advice -->

Encode elapsed time with segment-length ticks when readers must locate a time value on a simple 2D trajectory. For example, add repeated time ticks along a straight or smoothly curved path instead of using a monotone color gradient to show elapsed time.

## Why time ticks work <!-- role: reason -->

Tick spacing and tick count expose elapsed time more directly than subtle color changes along the path. This makes intermediate time positions easier to place without relying on fine discrimination of nearby color shades.

**Mechanism:** Segment-length ticks externalize equal time units on the path, so readers can judge elapsed time from the distribution of intervals instead of estimating it from a continuous color ramp.

**Evidence:** In the elapsed-time task on simple straight and smoothly curved 2D+time trajectories, length-based time encoding ranked above color-based time encoding in accuracy, and the paper explicitly recommends segment length for time while discouraging time-by-value encoding [@perinAssessingGraphicalPerception2018; @zengReviewCollationGraphical2023].

**Notes:** The reported ranking applies to time flattened onto a 2D path where time is not mapped to x or y.

## Use when the path must support exact time reading <!-- role: context -->

- **User Goal:** Locate an elapsed-time point on the path.
- **Task:** Place an intermediate time value such as an early, middle, or late point along the trajectory.
- **Data:** Ordered time is encoded on a 2D trajectory.
- **Chart Setting:** A static straight or smoothly curved path with no sharp angles, loops, or crossings.
- **Audience:** Readers making quick perceptual judgments rather than manual measurements.
- **Success Criterion:** More accurate placement of elapsed-time positions on the path.

## Do not use when the tested path conditions do not hold <!-- role: exceptions -->

- **Break it when:** The path has sharp corners, loops, crossings, or other complex geometry rather than a straight or smoothly curved form. **Why:** The encoding ranking was established only for very simple trajectories.
- **Break it when:** The time encoding also needs to show direction along the path. **Why:** Segment-length ticks convey elapsed time and inferred speed, but they do not provide direction.

## Costs of time ticks <!-- role: costs -->

**Sacrifice:** You add repeated marks to the path.
**Risk:** The ticks can take slightly longer to read than a direct color gradient and can visually compete with other line work.
**Mitigation:** Use them where the path and surrounding background keep the tick intervals visually distinct.

## Common failure mode: time by color gradient <!-- role: mistakes -->

**Mistake:** Use a continuous time color gradient when readers need an exact elapsed-time location on the path. **Why it fails:** Small color differences are hard to discriminate, so color-based time encoding produced larger errors than tick-based time encoding.

## Review check for elapsed-time encoding <!-- role: check -->

**Failure Sign:** Reviewers hesitate or guess when asked to place an intermediate elapsed-time point on the path.
**Quick Check:** Show the same simple trajectory once with time ticks and once with a time color gradient, then ask a reviewer to place the same elapsed-time point in both versions.
**Stronger Test:** Repeat that comparison with both a straight path and a smoothly curved path and keep the ticked version if it is more accurate in both.

## Fix the time encoding <!-- role: fix -->

- Replace the elapsed-time color gradient with repeated time ticks along the path.
- Keep the ticks perpendicular to the path so the segment spacing remains legible.
- If speed is also shown, keep time on the ticks rather than moving time to color shading.
