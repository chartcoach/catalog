---
id: use-categorical-hues-for-unordered-categories
title: Use a categorical hue scale for categories without intrinsic order
bibliography: references.bib
description: For comparing unordered groups, use color hues on categorical data to
  improve fidelity and mitigate false ordering for readers distinguishing categories.
labels:
- purpose:refine
- basis:heuristic
- data:categorical
- quality:fidelity
- lever:encoding
- channel:color-hue:use
---

## Use hues for unordered categories <!-- role: advice -->

Use distinct hues when color encodes categories that do not have an intrinsic order. For example, assign different hues to groups such as places, ethnicities, genders, or industries instead of using a light-to-dark gradient.

## Why unordered categories need hues <!-- role: reason -->

Categorical hues separate identities without implying rank. Readers can tell categories apart while understanding that no color means more or less than another.

**Mechanism:** Different hues signal distinct groups, not magnitude, so readers do not infer a low-to-high progression where none exists.

**Evidence:** The article recommends hues for categories without intrinsic order and states that categorical colors communicate that no category is worth more or less than the others [@muth_which_color_scale_2021].

## Use when the categories have no rank <!-- role: context -->

- **User Goal:** Distinguish groups from one another.
- **Task:** Compare categories as different identities, not as higher or lower values.
- **Data:** The color-encoded field is categorical and unordered.
- **Chart Setting:** Color is being used to encode that categorical field.
- **Audience:** Readers who need to tell categories apart without inferring magnitude.
- **Success Criterion:** The chart clearly separates groups without suggesting an order.

## Do not use when the values are ordered <!-- role: exceptions -->

**Break it when:** The color-encoded values have an intrinsic order or a meaningful middle value. **Why:** Hues communicate difference without more-or-less direction.

## Tradeoffs of categorical hues <!-- role: costs -->

**Sacrifice:** The palette does not communicate low-to-high magnitude.
**Risk:** Applying hues to ordered values removes the sense of progression.
**Mitigation:** Switch to a sequential or diverging gradient when the data needs ordered reading.

## Common ordering mistake <!-- role: mistakes -->

**Mistake:** Use unrelated hues for values such as income, temperature, or age. **Why it fails:** Readers cannot read the colors as a progression from lower to higher values.

## Check whether the field is truly unordered <!-- role: check -->

**Failure Sign:** The legend labels can be arranged naturally from lower to higher or from one side of a midpoint to the other.
**Quick Check:** Ask whether one category should be seen as more or less than another; if yes, do not use categorical hues.
**Stronger Test:** If readers need the colors alone to imply progression, replace the hue scale with a gradient.

## Fix the scale type <!-- role: fix -->

- Replace the gradient with distinct hues when the color-encoded field is unordered.
- Keep one hue per category rather than stepping light-to-dark through the same color family.
- Switch to a sequential or diverging scale if the field turns out to be ordered.
