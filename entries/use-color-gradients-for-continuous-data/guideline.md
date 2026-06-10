---
id: use-color-gradients-for-continuous-data
title: Use an ordered color gradient for continuous data
bibliography: references.bib
description: For comparing low-to-high values, use an ordered color gradient on quantitative
  color encodings to improve fidelity and mitigate false category cues for readers
  interpreting continuous data.
labels:
- purpose:refine
- basis:heuristic
- data:quantitative
- quality:fidelity
- lever:encoding
- polish:palette
---

## Use an ordered color gradient <!-- role: advice -->

Encode continuous data with an ordered color gradient instead of unrelated distinct hues. For example, color a rate map with light-to-dark steps that read as slightly lower or higher than neighboring steps, not with separate green, yellow, and blue category colors.

## Why ordered gradients work for continuous values <!-- role: reason -->

Ordered gradients make neighboring colors feel connected. That helps readers read color as a progression from lower to higher values instead of as separate groups.

**Mechanism:** A gradient signals that each color represents a value a bit higher or lower than the color next to it, so the color scale matches the structure of continuous data.

**Evidence:** The post says continuous data should use color gradients and explains that the colors in a gradient should communicate “I represent a value that’s a bit higher or lower than the color next to me,” using a map of unemployment rates as the example [@muth_colorguide_2018].

## Use when color must show ordered magnitude <!-- role: context -->

- **User Goal:** Show how values progress from low to high.
- **Task:** Let readers interpret magnitude from color.
- **Data:** Continuous or ordered numeric values.
- **Chart Setting:** A chart or map uses color as the main value encoding across many marks.
- **Audience:** Readers need to compare values by color without extra explanation.
- **Success Criterion:** Adjacent colors read as ordered steps of one scale.

## Do not use when the data is categorical <!-- role: exceptions -->

**Break it when:** The data consists of categories with no inherent order. **Why:** A gradient suggests adjacency and progression, which the source reserves for continuous data.

## Tradeoffs of ordered gradients <!-- role: costs -->

**Sacrifice:** You give up the strong separation that independent category hues provide.\
**Risk:** If the gradient is badly chosen, readers may not see clear steps between values.\
**Mitigation:** Keep the gradient but make neighboring steps more distinct.

## Common misuse of ordered gradients <!-- role: mistakes -->

**Mistake:** Using several unrelated hues to encode one low-to-high variable. **Why it fails:** The colors look like separate categories instead of parts of one ordered scale.

## Check whether the scale reads as a progression <!-- role: check -->

**Failure Sign:** The colors do not look like one ordered sequence.\
**Quick Check:** Ask whether each color could be described as slightly higher or lower than the one next to it.\
**Stronger Test:** Compare the gradient with a distinctive-hue version and keep the option that preserves the low-to-high reading.

## Fix the palette choice <!-- role: fix -->

- Replace unrelated category hues with a single ordered gradient.
- Arrange the colors so neighboring steps imply incremental change.
- Recheck the scale on the chart or map where it will be used.
