---
id: use-area-over-color-saturation-when-primary-quantitative-field-cannot-use-position
title: Use area instead of color-saturation when the primary quantitative field cannot
  use position
bibliography: references.bib
description: For multivariate point-based views where the primary quantitative field
  cannot use position, prefer area on the primary field to improve fidelity and mitigate
  higher decoding error from color-saturation for readers interpreting the main measure.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity:use
- lever:encoding
- measure:multi
- channel:area:use
- channel:color-saturation:avoid
---

## Put the primary quantitative field in area, not color-saturation <!-- role: advice -->

Use area instead of color-saturation when the main quantitative field cannot be placed on x or y in a point-based multivariate view. For example, if the other fields already occupy the positional channels, vary mark area for the main quantitative field rather than mapping that field to color-saturation.

## Why area is the better fallback <!-- role: reason -->

When the main measure had to leave position, area decoding produced fewer errors than color-saturation in the study. It is still a fallback, but it is the better of the two tested non-positional choices for the main quantitative field.

**Mechanism:** Area preserves more reliable reading of the main quantitative field than color-saturation when position is unavailable.

**Evidence:** The study reports that designs using area for the primary quantitative field performed better than the corresponding designs using color-saturation for that field across tasks, with lower error rates overall [@zengReviewCollationGraphical2023; @kimAssessingEffectsTask2018].

**Notes:** Position remained the strongest choice overall when it was available for the primary field.

## Use only when position is unavailable <!-- role: context -->

- **User Goal:** Preserve readability of the main quantitative field in a multivariate point-based view.
- **Task:** Any of the studied tasks where the same field remains the primary quantitative target.
- **Data:** One primary quantitative field, one secondary quantitative field, and one categorical field.
- **Chart Setting:** The primary quantitative field cannot be assigned to x or y because those channels are already committed.
- **Success Criterion:** Lower error on the primary field than a color-saturation fallback.

## Do not use this when a positional encoding is still possible <!-- role: exceptions -->

**Break it when:** The primary quantitative field can still be moved to x or y. **Why:** Position-based encodings ranked above both area and color-saturation for the primary field.

## What you give up <!-- role: costs -->

**Sacrifice:** You still give up the precision of a positional encoding.
**Risk:** Treating area as a full substitute for position can still leave exact reading weaker than the best positional designs.
**Mitigation:** Use area only as the fallback after ruling out x or y for the primary field.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Put the primary quantitative field on color-saturation after the positional channels are taken. **Why it fails:** That choice produced more decoding error than using area for the same field.

## Compare the fallback encodings <!-- role: check -->

**Failure Sign:** The main quantitative field is hard to decode once it leaves position.
**Quick Check:** Make two versions that differ only in whether the primary field uses area or color-saturation.
**Stronger Test:** Compare error on a few representative tasks before keeping the non-positional fallback.

## Change the fallback channel <!-- role: fix -->

- Remap the primary quantitative field from color-saturation to area.
- Keep the other fields on their existing channels.
- Reconsider the full field-to-channel assignment if exact reading of the primary field remains critical.
