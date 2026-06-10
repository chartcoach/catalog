---
id: use-color-saturation-instead-of-hue-for-ordered-color-scales
title: Use color saturation instead of color hue for ordered color scales
bibliography: references.bib
description: For ordered-value reading, prefer color saturation on continuous color
  encoding to improve fidelity and mitigate value misordering for viewers who infer
  order from color alone.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity:use
- lever:encoding
- polish:palette
- channel:color-saturation:use
- channel:color-hue:avoid
---

## Ordered color channel <!-- role: advice -->

Use a saturation-based ordered color ramp when color must carry low-to-high value order. For example, use a continuous saturation progression for quantitative or ordinal values instead of a hue-only sweep when readers must sort values directly from the palette.

## Why ordered saturation works <!-- role: reason -->

Hue-only ordered scales can change direction perceptually even when the numeric scale moves in one direction. That makes some colors hard to place between their neighbors and weakens direct ordering from color alone.

**Mechanism:** A monotonic ordered ramp keeps the perceived sequence moving in one direction, so adjacent and sampled colors are easier to place from low to high without repeated legend consultation.

**Evidence:** The collated review records this paper as guidance about using color hue and color saturation for ordered color encoding, and the paper explains that hue is difficult to order while ordered continuous ramps are evaluated by legend-based and intuitive order rather than by hue variety alone [@zengReviewCollationGraphical2023; @bujackGoodBadUgly2018].

## Use when value order must come from color <!-- role: context -->

- **User Goal:** Infer low-to-high order directly from color.
- **Task:** Sort or place sampled colors on an ordered scale.
- **Data:** Quantitative or ordinal values mapped to a continuous color scale.
- **Chart Setting:** Static display where readers may not continuously rely on the legend.
- **Audience:** Viewers who need the palette itself to communicate ordering.
- **Success Criterion:** Readers can place sampled colors in the correct order with little ambiguity.

## Do not use when legend lookup is enough <!-- role: exceptions -->

**Break it when:** Readers can rely on the legend for decoding and do not need to infer order directly from the colors themselves. **Why:** The paper separates intuitive order from legend-based order, so direct perceptual ordering is not always required.

## Tradeoffs of ordered saturation <!-- role: costs -->

**Sacrifice:** You may give up some of the wide color variation that high-hue sweeps provide.
**Risk:** A more ordered ramp can feel less globally discriminative if adjacent steps are compressed.
**Mitigation:** Check that neighboring colors still differ clearly while preserving a single perceptual direction.

## Common failure with hue sweeps <!-- role: mistakes -->

**Mistake:** Using a hue-only sweep for ordered values and expecting readers to sort colors correctly without the legend. **Why it fails:** Some palette regions do not preserve intuitive order, so the middle color in a sampled set may not look like the middle value.

## Check color order directly <!-- role: check -->

**Failure Sign:** Readers hesitate or disagree about which of three sampled colors is the middle value.
**Quick Check:** Sample three colors from the scale and ask whether one clearly reads as between the other two.
**Stronger Test:** Compute the minimal triangle-side difference over sampled triples; negative values indicate failed intuitive order.

## Fix hue-based misordering <!-- role: fix -->

- Replace the hue-only sweep with a monotonic saturation progression.
- Remove palette reversals or inflection points that break the low-to-high sequence.
- Re-sample the scale and revise any segment where the middle sampled color does not read as between its neighbors.
