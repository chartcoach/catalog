---
id: map-larger-values-to-darker-colors-when-the-colormap-does-not-appear-to-vary-in-opacity
title: Map larger values to darker colors when the colormap does not appear to vary
  in opacity
bibliography: references.bib
description: For aggregate comparison, use dark-more scale order on quantitative colormap
  views to improve interpretation speed and mitigate background-driven ambiguity for
  viewers reading with a legend.
labels:
- purpose:refine
- basis:empirical
- task:compare
- data:quantitative
- quality:readability:use
- lever:scale-order
- channel:color-lightness:use
---

## Dark-more scale order <!-- role: advice -->

Reverse the color scale so larger values map to darker colors when the scale does not look like a foreground fading into the background. For example, keep dark-more ordering on sequential colormaps that stay visually distinct from white or black backgrounds instead of flipping to light-more just because the background is dark.

## Why dark-more order works here <!-- role: reason -->

When the colormap does not appear to vary in opacity, readers rely on a dark-is-more cue rather than on background contrast. Aligning the legend with that cue reduces the time needed to interpret which side or region has more.

**Mechanism:** Darker colors are inferred as larger quantities when the palette does not visually behave like changing opacity against the background.

**Evidence:** The collated results record faster aggregate judgments for dark-more versions of non-opacity-varying scales, and the paper summarizes this pattern as a background-independent dark-is-more bias when apparent opacity variation is absent [@zengReviewCollationGraphical2023; @schlossMappingColorMeaning2019].

**Notes:** The reported benefit is about response time under high overall accuracy.

## Use when all of these are true <!-- role: context -->

- **User Goal:** Compare which side, region, or block has more overall.
- **Task:** Aggregate comparison from a quantitative color field.
- **Data:** Quantitative values encoded by a sequential colormap.
- **Chart Setting:** A legend is present, and the palette does not appear to be a reference color fading into the current background.
- **Audience:** Viewers need to read the display quickly without relearning the color order.
- **Success Criterion:** Faster correct interpretation of which region is larger overall.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** The colormap appears to vary in opacity and is shown on a dark background. **Why:** The opaque-is-more cue can conflict with dark-is-more and remove the advantage of dark-more ordering.

## Tradeoffs of dark-more order <!-- role: costs -->

**Sacrifice:** You give up light-more reversals that may look visually stronger on some dark-background presentations.
**Risk:** If the scale actually looks like changing opacity against the background, dark-more ordering can become slower to interpret.
**Mitigation:** Keep dark-more only with palettes that do not appear to vary in opacity, or change the palette before changing the mapping.

## Common mistake with dark-more order <!-- role: mistakes -->

**Mistake:** Reversing a non-opacity-varying scale to light-more on a dark background to chase contrast alone. **Why it fails:** The study did not support a general light-is-more advantage from dark backgrounds; dark-more remained faster when opacity variation was not the active cue.

## How to review this decision <!-- role: check -->

**Failure Sign:** The lighter end of the scale is labeled as “more,” but the palette does not visually read as a foreground fading into the background.
**Quick Check:** Inspect the scale against its background. If it does not resemble a linear fade from a reference color into that background, keep dark-more as the default mapping.
**Stronger Test:** A/B test the same display with dark-more and light-more legend order and keep the darker-high version if viewers answer faster with similar accuracy.

## What to change <!-- role: fix -->

- Reverse the legend and scale so the darker end represents larger values.
- Replace a near-background fade with a palette that does not appear to vary in opacity on the current background.
- Keep the same dark-more ordering across light and dark presentations only when the palette remains non-opacity-varying in both.
