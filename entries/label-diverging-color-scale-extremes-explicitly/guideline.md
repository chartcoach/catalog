---
id: label-diverging-color-scale-extremes-explicitly
title: Label the extremes of a diverging color scale explicitly
bibliography: references.bib
description: For explanation in charts that use a diverging color scale, use explicit
  legend, title, or annotation labels on the color encoding to improve readability
  and address confusion about which color means which extreme for readers decoding
  a non-intuitive scale.
labels:
- purpose:refine
- basis:heuristic
- quality:readability
- lever:text-annotation
- component:legend:use
- communication:context
- polish:annotation
- aesthetic:color:use
---

## Make each endpoint explicit <!-- role: advice -->

Label a diverging color scale so readers can tell which color means the low end and which means the high end. For example, write the legend endpoints clearly, turn the title into a color key, or add annotations in the chart that remind readers what each extreme represents.

## Why explicit endpoint labels matter <!-- role: reason -->

Diverging colors do not inherently tell readers which hue is high or low. Direct labels and reminders replace guessing with explicit meaning.

**Mechanism:** Endpoint labels anchor each side of the palette to a named extreme, so viewers do not have to infer the direction of the scale from hue alone.

**Evidence:** The article says diverging color scales are not intuitive, that readers need a color key, and recommends labeling the color legend well, turning the title into a color key, and using annotations to remind readers what they see [@muth_diverging_vs_sequential_2021].

## Use when a diverging scale is already chosen <!-- role: context -->

- **User Goal:** Help readers decode a diverging scale correctly.
- **Task:** Explain which side of the scale is low or high, better or worse.
- **Data:** Quantitative values already encoded with a diverging color scale.
- **Chart Setting:** The chart includes a legend, title, or annotations that can carry the mapping.
- **Audience:** Readers may not infer the direction of the hues on their own.
- **Success Criterion:** Readers can identify what each endpoint color means without hesitation.

## Do not use this as a substitute for a simpler scale <!-- role: exceptions -->

**Break it when:** A sequential light-to-dark scale already matches the intended message and reads intuitively. **Why:** The extra decoding support is mainly needed for diverging colors.

## Costs of explicit decoding support <!-- role: costs -->

**Sacrifice:** You spend extra space and attention on labels.\
**Risk:** Vague labels still leave the direction ambiguous.\
**Mitigation:** Name each extreme directly in the legend, title, or annotation.

## Common endpoint-labeling failure <!-- role: mistakes -->

**Mistake:** Using a diverging palette but leaving the endpoints implied. **Why it fails:** Viewers can invert the meaning of the colors.

## Check whether readers know what each color means <!-- role: check -->

**Failure Sign:** People pause over whether a color means more or less.\
**Quick Check:** Cover the numeric values and ask what each endpoint hue means; if the answer is uncertain, the scale is under-labeled.\
**Stronger Test:** Verify that the legend, title, or annotations explicitly name both extremes.

## Fix an ambiguous diverging scale <!-- role: fix -->

- Add clear endpoint labels to the legend for the low and high ends of the scale.
- Rewrite the title so it carries the same low-versus-high cue as the legend.
- Add brief annotations near colored marks to restate what the endpoints mean.
