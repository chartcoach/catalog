---
id: use-pair-preference-weighted-hue-palettes-when-palette-liking-is-the-main-goal
title: Use pair-preference-weighted hue palettes when palette liking is the main goal
bibliography: references.bib
description: For categorical palette design when palette liking is the main goal,
  prefer a pair-preference-weighted hue palette on nominal color encodings to maximize
  aesthetics and address harsh category combinations for readers judging the palette
  as a whole.
labels:
- purpose:refine
- basis:empirical
- data:categorical
- quality:aesthetics:use
- lever:encoding
- channel:color-hue:use
- aesthetic:color:use
---

## Weight the palette toward pair preference <!-- role: advice -->

Use a categorical hue palette that gives explicit weight to Pair Preference when viewer liking matters more than aggregate-reading accuracy. For example, choose a preference-weighted palette for a nominal color display when you want the palette itself to be rated more favorably, rather than choosing a low-error palette optimized for fast target-color comparisons.

## Why pair preference works <!-- role: reason -->

Pair Preference captures a consistent liking pattern for color combinations. Raising that weight makes the palette more appealing as a whole, even though it can weaken the separation needed for accurate count comparisons.

**Mechanism:** A pair-preference-weighted palette favors combinations people tend to like more, so the palette is judged more positively as a whole.

**Evidence:** The collated review includes this paper as nominal color-hue evidence. In the paper, upweighting Pair Preference made palettes more preferable on average, and the most preferable settings produced higher preference ratings than low-error settings in important size conditions, even though the tradeoff with discrimination remained. [@zengReviewCollationGraphical2023; @gramazioColorgoricalCreatingDiscriminable2017]

## Use when all of these are true <!-- role: context -->

- **User Goal:** Increase how much viewers like the palette.
- **Task:** Judge the palette as a color combination, not just count target-colored marks.
- **Data:** Nominal categories are encoded by hue.
- **Chart Setting:** The same palette will be seen across many marks or regions, and overall visual impression matters.
- **Audience:** Viewers are expected to react to the palette as a whole.
- **Success Criterion:** Higher preference ratings or stronger aesthetic approval.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** Readers must quickly and accurately decide which side, area, or group contains more of a target category. **Why:** Pair-preference-heavy palettes tended to worsen discrimination performance even while improving liking.

## Costs of weighting toward pair preference <!-- role: costs -->

**Sacrifice:** Some discrimination accuracy and speed.
**Risk:** The palette can become harder to use for target-versus-distractor judgments.
**Mitigation:** Rebalance some weight back toward discrimination if the palette will also support aggregate comparisons.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Using a pair-preference-heavy palette for a timed target-color comparison task. **Why it fails:** The palette can be liked more while still making the underlying color judgment less reliable.

## How to test the palette choice <!-- role: check -->

**Failure Sign:** Viewers like the palette, but they make more mistakes on target-color comparison tasks.
**Quick Check:** Compare the current preference-weighted palette against a more discrimination-weighted version on the same display and see whether the liking gain is paired with higher error.
**Stronger Test:** Run both a preference rating and an aggregate color comparison on the same candidate palettes and keep the preference-weighted version only if the aesthetic gain is worth the discrimination loss.

## What to change <!-- role: fix -->

- Increase Pair Preference weight when generating the nominal hue palette.
- Compare the preference-weighted palette against a low-error version instead of evaluating it in isolation.
- If confusion appears in use, shift some weight back toward discrimination and retest.
