---
id: use-diverging-color-scale-when-both-extremes-matter
title: Use a diverging color scale when the story depends on both extremes
bibliography: references.bib
description: For extreme-value emphasis in quantitative color-encoded charts, use
  a diverging color scale on data where both low and high ends matter to improve insight
  and address one-sided emphasis on only the highest values for readers scanning extremes.
labels:
- purpose:refine
- basis:heuristic
- task:extreme
- data:quantitative
- quality:insight
- lever:encoding
- communication:framing
- aesthetic:color:use
---

## Use color to highlight both tails <!-- role: advice -->

Use a diverging color scale when the story needs the lowest and highest values to stand out together. For example, replace a sequential light-to-dark map that mainly spotlights the highest values with a diverging map that also brings very low values into focus.

## Why diverging scales spotlight both ends <!-- role: reason -->

A sequential ramp naturally concentrates attention on its darkest end. A diverging ramp gives visual weight to both tails, so low values no longer disappear into a pale continuation of the same gradient.

**Mechanism:** Two opposing color directions make both extremes salient instead of giving the strongest emphasis to only one end.

**Evidence:** The article describes sequential versus diverging as an editorial choice: sequential scales support stories about the highest values, while diverging scales support stories about the lowest and highest values and bring low values into focus [@muth_diverging_vs_sequential_2021].

## Use when both extremes are part of the message <!-- role: context -->

- **User Goal:** Emphasize both tails of a quantitative distribution.
- **Task:** Highlight extremes rather than only rank the top end.
- **Data:** Quantitative values spread across low and high ends.
- **Chart Setting:** A chart or map already using a quantitative color scale.
- **Audience:** Readers are scanning for where the extremes are, especially at the low end.
- **Success Criterion:** Both low and high values are visually noticeable.

## Do not use when only the high end matters <!-- role: exceptions -->

**Break it when:** The message is mainly about the highest values. **Why:** A sequential scale emphasizes that single end more directly.

## Costs of emphasizing both tails <!-- role: costs -->

**Sacrifice:** You lose some of the simple one-ended emphasis of a sequential ramp.\
**Risk:** The low end may draw more attention than intended.\
**Mitigation:** Use a sequential scale if the message is only about the high end.

## Common extreme-emphasis failure <!-- role: mistakes -->

**Mistake:** Keeping a sequential scale when the intended message is about both low and high extremes. **Why it fails:** The low end stays visually subdued.

## Check whether both tails are visible <!-- role: check -->

**Failure Sign:** Low values blend into the background while high values dominate.\
**Quick Check:** Compare sequential and diverging previews; if only the diverging version makes the low end clearly visible and that matches the story, use it.\
**Stronger Test:** Check whether both tails are easy to spot without reading exact numbers.

## Fix one-sided emphasis <!-- role: fix -->

- Replace the sequential ramp with a diverging ramp so each extreme gets its own side of the palette.
- Center the diverging scale on the middle point used in the story.
- Revert to a sequential scale if the message is only about the top end.
