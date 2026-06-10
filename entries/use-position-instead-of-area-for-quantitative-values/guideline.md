---
id: use-position-instead-of-area-for-quantitative-values
title: Use position instead of area to encode quantitative values
bibliography: references.bib
description: For exact value reading in static charts with quantitative data, prefer
  position encoding on a chosen chart to improve fidelity and mitigate misread magnitudes
  for readers comparing numeric values.
labels:
- purpose:refine
- basis:empirical
- data:quantitative
- quality:fidelity
- lever:encoding
- reading-mode:exact
- channel:position:use
- channel:area:avoid
---

## Position encoding for the main numeric field <!-- role: advice -->

Encode the main quantitative field with x or y position instead of area when accurate numeric reading matters. For example, place the value on an axis rather than sizing points or bubbles by that same value.

## Why position works better than area here <!-- role: reason -->

Position on an axis gives readers a more accurate perceptual readout of numeric magnitude than judging marked area. Moving the main value to position reduces reliance on a weaker magnitude judgment.

**Mechanism:** Position supports more accurate quantitative interpretation than area for the same field.

**Evidence:** The collated knowledge records Mackinlay's quantitative effectiveness ranking as positionX = positionY > length > angle > orientation > area > color-saturation > color-hue, so position is the stronger encoding choice over area for quantitative data [@zengReviewCollationGraphical2023; @mackinlayAutomatingDesignGraphical1986].

**Notes:** PositionX and positionY are tied in the recorded ranking.

## Use when quantitative accuracy is the goal <!-- role: context -->

- **User Goal:** Read or compare numeric values accurately.
- **Data:** One quantitative field is being assigned to a visual channel.
- **Chart Setting:** A static 2D chart is being designed, and the same field could be mapped to either position or area.
- **Success Criterion:** The value can be interpreted more accurately from the graphic itself.

## Do not use when the field is not quantitative <!-- role: exceptions -->

**Break it when:** The field is ordinal or categorical rather than quantitative. **Why:** This ranking is explicitly recorded for quantitative encodings.

## Costs of moving the field to position <!-- role: costs -->

**Sacrifice:** Position uses an axis slot.
**Risk:** Forcing every field onto position can crowd out more important information in a multivariate design.
**Mitigation:** Keep the most important field on position and move a less important field to a lower-ranked channel.

## Common failure around this choice <!-- role: mistakes -->

**Mistake:** Keep the main quantitative field on area-sized marks when an axis position mapping is available. **Why it fails:** It leaves readers judging area instead of the higher-ranked position task.

## Check the encoding decision directly <!-- role: check -->

**Failure Sign:** Readers must compare bubble sizes or other areas to answer numeric questions.
**Quick Check:** Redraw the same field on x or y position and see whether the reading no longer depends on size judgments.
**Stronger Test:** If the positioned version expresses the same field, keep the position mapping and remove area from the main quantitative field.

## Fix the channel assignment <!-- role: fix -->

- Move the quantitative field to x or y position.
- Replace variable-sized marks with equal-sized marks when area no longer carries the main value.
- If another field still needs encoding, assign the less important field to area instead of the main quantitative field.
