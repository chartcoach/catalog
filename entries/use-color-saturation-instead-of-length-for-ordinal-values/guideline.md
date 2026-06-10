---
id: use-color-saturation-instead-of-length-for-ordinal-values
title: Use color saturation instead of length to encode ordinal values
bibliography: references.bib
description: For ordered-level reading in static charts with ordinal data, prefer
  color saturation encoding on a chosen chart to improve fidelity and mitigate weak
  progression judgments for readers interpreting ranked levels.
labels:
- purpose:refine
- basis:empirical
- data:ordinal
- quality:fidelity
- lever:encoding
- channel:color-saturation:use
- channel:length:avoid
---

## Saturation encoding for ordered levels <!-- role: advice -->

Encode the ordinal field with color saturation instead of length when the goal is to show ordered levels. For example, use progressively stronger saturation for ranked categories rather than different bar or segment lengths for that same ordered field.

## Why saturation works better than length here <!-- role: reason -->

Ordinal data asks readers to recover order rather than exact numeric magnitude. Using saturation for the ordered field aligns the encoding with a higher-ranked ordinal perceptual task than length.

**Mechanism:** Color saturation supports more effective ordinal interpretation than length for the same ordered field.

**Evidence:** The collated knowledge records Mackinlay's ordinal effectiveness ranking as positionX = positionY > color-saturation > color-hue > texture > length > angle > orientation > area, so color saturation is the stronger encoding choice over length for ordinal data [@zengReviewCollationGraphical2023; @mackinlayAutomatingDesignGraphical1986].

## Use when order matters more than numeric magnitude <!-- role: context -->

- **User Goal:** Show ranked levels or ordered progression.
- **Data:** One ordinal field is being assigned to a visual channel.
- **Chart Setting:** A static 2D chart is being designed, and the same field could be mapped to either color saturation or length.
- **Success Criterion:** Readers can recover the intended order more effectively from the graphic.

## Do not use when the field is not ordinal <!-- role: exceptions -->

**Break it when:** The field is quantitative or nominal rather than ordinal. **Why:** This ranking is explicitly recorded for ordinal encodings.

## Costs of moving the field to saturation <!-- role: costs -->

**Sacrifice:** Saturation uses the color channel.
**Risk:** If position is still available for the same ordered field, stopping at saturation leaves a higher-ranked option unused.
**Mitigation:** Use saturation when the chosen design is not giving that field a position channel.

## Common failure around this choice <!-- role: mistakes -->

**Mistake:** Keep the ordinal field on length when the message is ordered level rather than exact quantity. **Why it fails:** It uses a lower-ranked ordinal channel than saturation.

## Check the encoding decision directly <!-- role: check -->

**Failure Sign:** Ordered levels are carried by different lengths even though a saturation mapping is available.
**Quick Check:** Remap the same ordered field to stepped saturation and see whether the order can be read without relying on lengths.
**Stronger Test:** If the saturation version still expresses the ordered levels, keep saturation and remove the length mapping from that field.

## Fix the channel assignment <!-- role: fix -->

- Replace the length mapping with a stepped saturation mapping for the ordinal field.
- Use a consistent length when length no longer carries the ordered field.
- If an axis becomes available for the most important ordered field, move that field to position.
