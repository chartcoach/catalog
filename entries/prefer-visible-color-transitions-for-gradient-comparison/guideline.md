---
id: prefer-visible-color-transitions-for-gradient-comparison
title: Prefer a palette with visible color transitions for gradient comparison
bibliography: references.bib
description: For side-by-side gradient comparison, prefer palette choices with visible
  color transitions on color-coded quantitative scalar fields to improve discrimination
  of net gradient differences and mitigate missed structural differences for viewers
  making overview judgments.
labels:
- purpose:refine
- basis:empirical
- task:compare
- data:quantitative
- quality:fidelity:use
- lever:encoding
- operator:difference
- polish:palette
---

## Palette choice for gradient comparison <!-- role: advice -->

Use a palette with visible color transitions when a color-coded scalar field must support side-by-side comparison of overall gradient. For example, replace a smooth monotonic-luminance palette such as viridis with a diverging cool-warm palette when viewers must judge which of two fields changes more steeply on average.

## Why visible transitions help <!-- role: reason -->

Visible color transitions create discrete regions that viewers can use as cues for how quickly values change across the field. That makes small structural differences in average gradient easier to discriminate.

**Mechanism:** A palette with stronger apparent boundaries makes changes in the field look more segmented, which supports overview comparison of net steepness between two maps.

**Evidence:** In the collated graphical-perception record, the aggregate-task JND ranking places the cool-warm design ahead of the viridis design, with a significant advantage for cool-warm over viridis. The original experiment reported lower JNDs for cool-warm than viridis for judging which scalar field had steeper average gradients, and this ordering held across the tested spatial-frequency levels [@zengReviewCollationGraphical2023; @redaEvaluatingGradientPerception2019].

**Notes:** The measured outcome was just-noticeable difference for average-gradient discrimination, where lower values indicate better sensitivity.

## Where this applies <!-- role: context -->

- **User Goal:** Decide which of two scalar fields has higher average gradient.
- **Task:** Compare an aggregate spatial property rather than read exact values at specific locations.
- **Data:** Two continuous quantitative scalar fields encoded with color.
- **Chart Setting:** Static side-by-side color-coded fields using the same palette family for the comparison.
- **Audience:** Viewers making perceptual comparison judgments without needing domain-specific training.
- **Success Criterion:** Readers can detect smaller differences in overall gradient.

## When not to use it <!-- role: exceptions -->

**Break it when:** The chart's main job is not comparing overall gradient between scalar fields. **Why:** The evidence is task-specific and only supports aggregate gradient judgments, not general-purpose color-map choice for other reading tasks.

## Costs of this choice <!-- role: costs -->

**Sacrifice:** You give up some visual smoothness in the color ramp.
**Risk:** If applied blindly outside gradient comparison, the visible transitions can act like artifacts instead of helpful cues.
**Mitigation:** Keep this palette choice tied to views whose primary job is comparing overall steepness.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep a smooth monotonic-luminance palette for a view whose main job is side-by-side gradient comparison. **Why it fails:** Readers need larger gradient differences before they can reliably tell which field is steeper.

## How to test it <!-- role: check -->

**Failure Sign:** Subtle differences in steepness disappear or readers hesitate when choosing between two fields.
**Quick Check:** Show the same field pair once with the current smooth palette and once with a cool-warm palette, then ask which field is steeper on average.
**Stronger Test:** Estimate the smallest gradient difference at which readers stay correct about three quarters of the time and compare that threshold across the two palette versions.

## What to change <!-- role: fix -->

- Replace the smooth monotonic-luminance palette in the comparison view with a diverging palette that has visible color transitions.
- Apply the revised palette consistently across both fields being compared.
- Re-test the revised view on field pairs with only subtle gradient differences to confirm that the comparison becomes easier.
