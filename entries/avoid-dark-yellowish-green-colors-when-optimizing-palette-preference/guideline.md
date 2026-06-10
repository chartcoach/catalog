---
id: avoid-dark-yellowish-green-colors-when-optimizing-palette-preference
title: Avoid dark yellowish-green colors when optimizing categorical palette preference
bibliography: references.bib
description: For aesthetic evaluation of categorical palettes, avoid dark yellowish-green
  hues on categorical color encodings to maximize aesthetics and mitigate disliked
  color-region choices for viewers judging palette appeal.
labels:
- purpose:refine
- basis:empirical
- data:categorical
- quality:aesthetics
- lever:encoding
- polish:palette
- aesthetic:color:avoid
- channel:color-hue:avoid
---

## Filter the disliked yellow-green region <!-- role: advice -->

Remove dark yellowish-green colors when average viewer preference matters. For example, avoid hues around 85°–114° with lightness around 35–75, and penalize nearby yellow-green colors that border this region.

## Why this region hurts preference <!-- role: reason -->

A preference-driven palette can drift into disliked yellow-green colors when cool blues and strong separation are both rewarded. Filtering that region keeps the palette from solving discriminability by introducing colors that people tend to dislike.

**Mechanism:** Preference weighting pulls toward cool blues, and discrimination weighting can then push their opposites toward darker yellows; filtering the dark yellowish-green region blocks that undesirable path.

**Evidence:** The paper excludes a dark yellowish-green region because those colors are generally disliked on average, and reports that removing this region still preserved enough color space for discriminable pairings while improving typical palette preference [@gramazioColorgoricalCreatingDiscriminable2017].

**Notes:** The paper also adds a penalty for nearby yellow-green candidates so border cases are sampled less often.

## Use when optimizing for average viewer preference <!-- role: context -->

- **User Goal:** Raise average palette appeal.
- **Task:** Generate or revise a categorical palette that must balance preference with discrimination.
- **Data:** Categorical groups encoded by color.
- **Chart Setting:** A palette that includes blues or other colors that could otherwise drive selection toward dark yellow opposites.
- **Audience:** A broad audience whose average preference matters more than individual taste.
- **Success Criterion:** Fewer disliked yellow-green colors without losing usable category separation.

## Do not use when a known audience specifically wants those colors <!-- role: exceptions -->

**Break it when:** The design is for a known observer or audience that specifically prefers these yellow-green colors. **Why:** The paper notes individual differences and that some observers may like them even though they are generally disliked on average.

## Filtering the region reduces some available contrasts <!-- role: costs -->

**Sacrifice:** You lose part of the yellow-green color space.
**Risk:** If applied blindly, you may remove some otherwise discriminable oppositions against blues.
**Mitigation:** Keep using other yellow regions outside the filtered dark zone.

## Common yellow-green failure <!-- role: mistakes -->

**Mistake:** Letting discriminability and coolness push the palette toward dark yellow opposites of selected blues. **Why it fails:** That interaction produces colors the paper identifies as generally disliked.

## Inspect the hue-lightness region directly <!-- role: check -->

**Failure Sign:** The palette contains muddy dark yellow-greens that feel noticeably less appealing than the other colors.
**Quick Check:** Check whether any palette color falls in the hue range 85°–114° and the lightness range 35–75.
**Stronger Test:** Compare the current palette against a version with those colors replaced and collect preference ratings.

## Replace or penalize the filtered region <!-- role: fix -->

- Replace colors inside the filtered region with nearby colors outside it.
- Penalize neighboring yellow-green candidates so the palette generator samples them less often.
- Regenerate the palette and keep the version with the higher minimum pair preference.
