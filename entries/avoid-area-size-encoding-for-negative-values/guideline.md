---
id: avoid-area-size-encoding-for-negative-values
title: Avoid area-size encoding for negative values
bibliography: references.bib
description: For quantitative reading with signed values, avoid area encoding on charts
  with sized marks to improve fidelity and mitigate larger-means-more misreadings
  for readers.
labels:
- purpose:refine
- basis:empirical
- data:quantitative
- quality:fidelity:use
- lever:encoding
- channel:area:avoid
---

## Area-size encoding removal <!-- role: advice -->

Do not use mark area to encode a signed measure. For example, avoid bubbles or sized circles when values can fall below zero, because larger areas still read as larger quantities.

## Why area breaks on negative values <!-- role: reason -->

Area works as a quantity metaphor only while bigger means more. Once the measure can go below zero, the size metaphor stops matching the meaning of the data.

**Mechanism:** Larger areas are firmly associated with larger positive amounts, so area cannot cleanly express both direction and magnitude for signed values.

**Evidence:** The paper states that area can convey quantity, but it cannot easily show negative values because larger sizes remain tied to larger positive quantities [@bertiniWhyShouldntAll2020].

## Use when the measure can cross zero <!-- role: context -->

- **User Goal:** Show a quantitative measure faithfully.
- **Task:** Read signed values, including negatives.
- **Data:** Numeric values that can be positive and negative.
- **Chart Setting:** The design is using or considering sized marks such as circles.
- **Audience:** Readers who need the sign as well as the magnitude.
- **Success Criterion:** The encoding does not make larger marks imply the wrong direction.

## Do not use this rule for non-negative magnitudes <!-- role: exceptions -->

**Break it when:** All encoded values are non-negative. **Why:** The larger-area-equals-larger-quantity metaphor still holds in that case.

## Costs of removing area-size encoding <!-- role: costs -->

**Sacrifice:** You give up a compact size-based display for that measure.
**Risk:** If you keep area for signed data, negative values can look like larger amounts rather than values below zero.
**Mitigation:** Move the signed field off area and reserve area for non-negative magnitude fields.

## Common sized-mark mistake <!-- role: mistakes -->

**Mistake:** Sizing marks by a value that can go negative. **Why it fails:** The display cannot keep the larger-means-more metaphor consistent across zero.

## Check whether area is invalid for the measure <!-- role: check -->

**Failure Sign:** The most negative values would require the largest marks or an impossible notion of negative size.
**Quick Check:** Ask whether the encoding can cross zero without breaking the size metaphor.
**Stronger Test:** If a larger mark ever stands for a smaller signed value, the area encoding has failed.

## Fix the signed-value encoding <!-- role: fix -->

- Remove area sizing from the signed field.
- Switch the signed field to a channel that can express both direction and magnitude.
- Keep area only for fields where larger always means more.
