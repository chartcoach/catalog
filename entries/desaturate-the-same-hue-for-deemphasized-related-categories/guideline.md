---
id: desaturate-the-same-hue-for-deemphasized-related-categories
title: De-emphasize related categories with a less saturated version of the same hue
bibliography: references.bib
description: For charts that highlight one category against related background marks,
  prefer lower saturation within the same hue on the background marks to improve hierarchy
  and mitigate false category breaks for readers who should read those marks as one
  family.
labels:
- purpose:refine
- basis:heuristic
- quality:fidelity
- lever:encoding
- polish:hierarchy
- aesthetic:color:use
- channel:color-saturation:use
- channel:color-hue:avoid
---

## Keep one hue family for deemphasis <!-- role: advice -->

Keep the hue constant and lower saturation on the less important marks. For example, show the focal line, points, or labeled marks in a strong blue and the background marks in a lighter, less saturated blue rather than in a different blue that reads like a separate category.

## Why same-hue desaturation preserves meaning <!-- role: reason -->

A new hue suggests a different kind of thing, not just a quieter version of the same thing. Lower saturation keeps the relationship intact while still pushing the background marks back.

**Mechanism:** Readers treat hue changes as category changes, but they treat saturation changes within one hue as a hierarchy inside one family.

**Evidence:** The post recommends sticking to gray or desaturation for de-emphasized categories, warns that another hue communicates a separate category, and shows a redesign where labeled and unlabeled points use the same hue with different saturation instead of two different hues [@muth_emphasize_color_2023].

## Use when related marks should stay in one family <!-- role: context -->

- **User Goal:** Highlight one set of marks without implying that the quieter marks belong to a different category.
- **Task:** De-emphasize related background marks while preserving their relationship to the highlighted marks.
- **Data:** Related categories, points, or series that should still be read as the same kind of mark.
- **Chart Setting:** A chart where some marks are labeled or foregrounded and others are background context.
- **Audience:** Readers should perceive one category family with different importance levels.
- **Success Criterion:** The quieter marks look related to the highlight, not like a separate grouping.

## Do not use when a true category difference is the message <!-- role: exceptions -->

**Break it when:** You want the background marks to be read as a genuinely separate category. **Why:** A different hue is useful when categorical difference, not simple deemphasis, is what readers need to see.

## Tradeoffs of same-hue desaturation <!-- role: costs -->

**Sacrifice:** You give up some palette variety.
**Risk:** If the background color is not clearly the same hue, the relationship becomes ambiguous.
**Mitigation:** Make the quieter color a straightforward less saturated version of the highlight color.

## Common failures in same-hue deemphasis <!-- role: mistakes -->

- **Mistake:** Introducing a new hue only to de-emphasize background marks. **Why it fails:** Readers infer a category break instead of a priority change.
- **Mistake:** Using a background color that is not simply a less saturated version of the highlight hue. **Why it fails:** The intended family relationship becomes unclear.

## Check whether the quieter marks still read as related <!-- role: check -->

**Failure Sign:** Background marks look like a second category instead of a weaker version of the highlighted one.
**Quick Check:** Compare the two swatches side by side and confirm that the quieter one is the same hue with less saturation.
**Stronger Test:** If you would describe the pair as two different colors rather than one stronger and one weaker version, the deemphasis is unclear.

## Fix hue-driven category breaks <!-- role: fix -->

- Replace the background color with a less saturated version of the highlight hue.
- Remove any extra hue that exists only to push background marks back.
- Keep labeled and unlabeled versions of the same kind of mark in one hue family.
