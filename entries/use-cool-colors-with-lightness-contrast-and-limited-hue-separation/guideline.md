---
id: use-cool-colors-with-lightness-contrast-and-limited-hue-separation
title: Use cool colors with lightness contrast and limited hue separation
bibliography: references.bib
description: For aesthetic evaluation of categorical palettes, use cool colors with
  lightness contrast and limited hue separation on categorical color encodings to
  maximize aesthetics and address disliked color pairings for viewers judging palette
  appeal.
labels:
- purpose:refine
- basis:empirical
- data:categorical
- quality:aesthetics
- lever:encoding
- polish:palette
- aesthetic:color:use
- channel:color-hue:use
- channel:color-lightness:use
---

## Tune palette preference cues <!-- role: advice -->

Favor cool colors, keep some lightness contrast, and avoid very large hue gaps when palette likability matters. For example, the supported preference model favors greener-bluer colors over orangish reds, prefers pairs with lightness differences, and assigns higher preference to relatively similar hues.

## Why these color relations feel better <!-- role: reason -->

Palette preference rises when the component colors fit the visual relations people tend to like as a combination. Coolness, lightness contrast, and limited hue separation work together to make categorical palettes more appealing.

**Mechanism:** Cool colors raise average liking, lightness contrast keeps pairs visually active, and smaller hue gaps make the combination feel more preferable as a whole.

**Evidence:** The palette preference model used in the paper predicts higher preference for cool colors, larger lightness contrast, and smaller hue differences, and palettes with higher Pair Preference scores were rated as more preferable by participants [@gramazioColorgoricalCreatingDiscriminable2017].

**Notes:** The paper distinguishes preference from traditional color-harmony rules and does not treat complementary hues as a reliable preference cue.

## Use when palette appeal is a design goal <!-- role: context -->

- **User Goal:** Make a categorical palette more aesthetically pleasing.
- **Task:** Choose among palette alternatives by how much viewers like them.
- **Data:** Categorical groups encoded by color.
- **Chart Setting:** A visualization where palette appeal matters alongside basic category separation.
- **Audience:** Viewers giving preference judgments or reacting to the palette as a whole.
- **Success Criterion:** Higher preference ratings for the palette.

## Do not use when discrimination speed and accuracy dominate <!-- role: exceptions -->

**Break it when:** Accurate and rapid category discrimination is more important than palette appeal. **Why:** Higher Pair Preference scores were associated with worse discrimination performance because preferable palettes tended to use more similar hues.

## Preference can trade off against separability <!-- role: costs -->

**Sacrifice:** You give up some discriminability.
**Risk:** Similar-hue palettes can become harder to tell apart, especially as the number of colors grows.
**Mitigation:** Compare the preferred palette against a more separated alternative if the chart also needs fast lookup.

## Common preference failure <!-- role: mistakes -->

**Mistake:** Using large complementary hue jumps as a shortcut to a “harmonious” palette. **Why it fails:** The paper notes that people often judge complementary hues as less harmonious and less preferable than more similar hues.

## Test preference against a nearby alternative <!-- role: check -->

**Failure Sign:** The palette feels harsh or is rated low in preference even though the colors are individually usable.
**Quick Check:** Inspect whether the palette relies heavily on warm hues, minimal lightness contrast, or very large hue gaps.
**Stronger Test:** A/B test the current palette against an alternative with a higher Pair Preference score and collect direct preference ratings.

## Adjust hue family and lightness contrast <!-- role: fix -->

- Replace some warm hues with cooler ones.
- Increase lightness differences between colors that currently sit at similar lightness levels.
- Reduce extreme hue gaps among colors that should feel like a coherent palette.
