---
id: use-segment-length-ticks-when-one-path-must-encode-both-time-and-speed
title: Use segment-length ticks when one path must encode both time and speed
bibliography: references.bib
description: For point lookup on ordered-time trajectories, use segment-length ticks
  on simple 2D path views to improve fidelity and mitigate loss of either time or
  speed when one encoding must carry both for readers inspecting the same path for
  both quantities.
labels:
- purpose:refine
- basis:empirical
- time:ordered-time
- quality:fidelity:use
- lever:encoding
- operator:lookup
- measure:multi
- channel:length:use
---

## Segment-length ticks for dual encoding <!-- role: advice -->

Use segment-length ticks when the same path must carry both elapsed time and local speed with one encoding. For example, divide the trajectory into repeated time units with perpendicular ticks so elapsed time comes from tick distribution and speed comes from the spacing between adjacent ticks, rather than asking one width encoding to do both jobs.

## Why one tick system can carry both quantities <!-- role: reason -->

A ticked path exposes two readings at once: the repeated intervals show elapsed time, and the gap between intervals reveals local speed. This avoids overloading width or color to stand in for both quantities on the same path.

**Mechanism:** Segment-length ticks provide an explicit time scaffold while also turning local segment spacing into a readable speed cue, so one encoding supports both questions on the same trajectory.

**Evidence:** On simple 2D+time trajectories, the paper recommends segment length whenever possible for conveying both time and speed, and specifically recommends segment length alone when only one visual variable is available [@perinAssessingGraphicalPerception2018; @zengReviewCollationGraphical2023].

**Notes:** The source also reports that adding speed color on top of segment length can further support reading when another channel is available.

## Use when one trajectory must answer both time and speed questions <!-- role: context -->

- **User Goal:** Read both elapsed time and local speed from the same path.
- **Task:** Locate time positions and identify speed extrema on one trajectory.
- **Data:** Ordered time and varying speed are both encoded on a 2D trajectory.
- **Chart Setting:** A static straight or smoothly curved path, with limited visual variables available for additional encoding.
- **Audience:** Readers making quick perceptual readings from a single path view.
- **Success Criterion:** One encoding supports both quantities with usable accuracy.

## Do not use when ticks cannot carry the full job <!-- role: exceptions -->

- **Break it when:** The path also needs the time encoding to indicate direction. **Why:** Segment-length ticks do not provide direction along the path.
- **Break it when:** Background lines or surrounding structure visually compete with the ticks. **Why:** Conflicting lines make the intervals harder to decode as time and speed cues.

## Costs of a tick-based dual encoding <!-- role: costs -->

**Sacrifice:** You add extra marks and visual density to the path.
**Risk:** The ticks can create clutter and may be slower to read than a single direct color ramp for a single question.
**Mitigation:** Use this approach when the constraint is carrying both quantities on one path and the tick marks remain visually separable.

## Common failure mode: one width encoding for two quantities <!-- role: mistakes -->

**Mistake:** Use one width-varying path to communicate both elapsed time and speed. **Why it fails:** Size-based double encodings underperformed the tick-based encoding and can obscure both readings.

## Review check for a dual encoding <!-- role: check -->

**Failure Sign:** Reviewers can answer either the time question or the speed question, but not both from the same path.
**Quick Check:** Show one ticked trajectory and ask a reviewer for both an elapsed-time point and the fastest or slowest point.
**Stronger Test:** Compare that ticked version against a width-only dual encoding on the same simple trajectory and keep the version that supports both answers more accurately.

## Fix the dual encoding <!-- role: fix -->

- Divide the path into repeated time units with perpendicular ticks.
- Let the spacing between neighboring ticks carry local speed instead of using width alone.
- If another channel becomes available later, keep the ticks and add speed color rather than replacing the ticks.
