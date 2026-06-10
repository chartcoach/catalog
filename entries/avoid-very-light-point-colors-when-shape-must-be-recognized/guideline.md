---
id: avoid-very-light-point-colors-when-shape-must-be-recognized
title: Avoid very light point colors when shape differences must be recognized
bibliography: references.bib
description: For shape recognition, avoid very light point colors on white-background
  scatterplots to prevent missed shape differences and address low point-to-background
  contrast for viewers distinguishing categories.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:scatter
- quality:fidelity:use
- lever:encoding
- channel:color-lightness:avoid
- channel:shape
---

## Lightness limits for shape reading <!-- role: advice -->

Avoid very light point colors when readers must tell point shapes apart on a white background. For example, do not push filled or open point symbols toward near-white values if shape itself encodes category, because shape recognition only degraded at the lightest tested colors.

## Why very light colors hide shape differences <!-- role: reason -->

Shape recognition depends on seeing the point boundary clearly. When the point color gets too close to the background lightness, fine geometric details become harder to resolve.

**Mechanism:** Very low contrast between the point and the background weakens edge visibility, which makes same/different shape judgments less reliable.

**Evidence:** The study found little to no interference from color on shape perception except for extremely light colors on the white background, where accuracy dropped only at the highest tested lightness values. The review collated this paper as evidence on shape-color interference in scatterplots [@smartMeasuringSeparabilityShape2019; @zengReviewCollationGraphical2023].

**Notes:** The paper reports this as a limited, asymptotic effect rather than a broad color problem.

## Use when shape carries category information <!-- role: context -->

- **User Goal:** Distinguish categories by point shape.
- **Task:** Decide whether two point shapes are the same or different.
- **Data:** Scatterplot data where shape is a meaningful encoding.
- **Chart Setting:** A white-background scatterplot with colored point marks.
- **Audience:** Readers identifying category symbols from point geometry.
- **Success Criterion:** Shape differences remain recognizable across the full color range.

## Do not use when point colors stay away from the background <!-- role: exceptions -->

**Break it when:** The point colors remain comfortably darker than the white background. **Why:** The paper found shape perception stayed stable outside the extremely light end of the tested range.

## Tradeoffs of avoiding the palest colors <!-- role: costs -->

**Sacrifice:** You use less of the palest part of a lightness range.
**Risk:** Near-white point colors can erase fine shape detail against the background.
**Mitigation:** Reserve the lightest colors for cases where shape is not the cue readers must distinguish.

## Common failure with shape-encoded points <!-- role: mistakes -->

**Mistake:** Using near-white point colors and assuming shape categories will stay as readable as darker colors. **Why it fails:** Accuracy dropped only when the marks approached the background lightness.

## How to review the lightness range <!-- role: check -->

**Failure Sign:** Readers hesitate or miss same/different shape judgments only for the palest colors.
**Quick Check:** Preview each candidate shape at the lightest planned color against the final background.
**Stronger Test:** A/B compare a lighter and darker version of the same shape set and keep the one with stable shape recognition.

## What to change <!-- role: fix -->

- Darken the lightest point colors until shape edges remain visible against the background.
- Re-test fine-detail shapes at the palest planned color, not just the midrange colors.
- Keep shape-carrying marks away from near-white values on white backgrounds.
