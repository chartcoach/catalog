---
id: separate-categorical-colors-by-perception-and-name
title: Separate categorical colors by both perception and name
bibliography: references.bib
description: For categorical comparison in information visualizations, use large perceptual
  and color-name separation on categorical color encodings to improve readability
  and address color-confusion errors for viewers distinguishing categories.
labels:
- purpose:refine
- basis:empirical
- task:compare
- data:categorical
- quality:readability
- lever:encoding
- polish:palette
- aesthetic:color:use
---

## Increase pairwise color separation <!-- role: advice -->

Increase both perceptual distance and color-name difference between categorical palette colors when viewers must tell categories apart quickly. For example, avoid pairs that still fall into the same broad named color family even if they look somewhat separated, and prefer palettes whose weakest pair has both high CIEDE2000 distance and high name difference.

## Why joint separation works <!-- role: reason -->

The hardest color pair in a palette limits how accurately people can identify categories. A palette becomes easier to use when its weakest pair is separated both by appearance and by the names people are likely to assign to those colors.

**Mechanism:** Perceptual distance reduces visual confusion, and color-name difference reduces confusion when two colors would otherwise be called by the same broad name.

**Evidence:** In human testing, response time and error generally improved as palette Perceptual Distance and Name Difference increased, and Name Difference was often the stronger predictor of discrimination behavior [@gramazioColorgoricalCreatingDiscriminable2017].

**Notes:** The paper explicitly treats the minimum pair score in a palette as the limiting case for discriminability.

## Use when palette discrimination is the job <!-- role: context -->

- **User Goal:** Distinguish color-coded categories accurately.
- **Task:** Compare or find categories by color.
- **Data:** Categorical groups encoded only by color.
- **Chart Setting:** A visualization where category colors may be glanced at quickly or referred to by broad color names.
- **Audience:** Viewers who need fast and accurate color discrimination.
- **Success Criterion:** Fewer color confusions, fewer errors, and faster responses.

## Do not use when preference matters more than discrimination <!-- role: exceptions -->

**Break it when:** Palette liking is the primary success criterion and some loss of discriminability is acceptable. **Why:** Greater perceptual and name separation tended to reduce preference ratings while more preferable palettes were often less discriminable.

## Weigh the discrimination gain against preference loss <!-- role: costs -->

**Sacrifice:** You give up some palette coherence and likability.
**Risk:** Pushing separation too hard can create palettes people like less.
**Mitigation:** If the chart also needs to feel appealing, compare the current palette against a slightly less separated alternative instead of maximizing separation blindly.

## Common separation failure <!-- role: mistakes -->

**Mistake:** Optimizing only perceptual distance or only color-name difference. **Why it fails:** The paper shows these are related but distinct signals, so a palette can still confuse viewers if one of them is weak.

## Review the weakest pair, not just the average palette <!-- role: check -->

**Failure Sign:** One color pair is repeatedly confused even though the rest of the palette looks acceptable.
**Quick Check:** Inspect the lowest-scoring pair in the palette and ask whether the two colors both look close and would likely receive the same broad name.
**Stronger Test:** A/B test the current palette against an alternative with a higher minimum pairwise perceptual and name-difference score on a short category-identification task.

## Edit the weakest pair first <!-- role: fix -->

- Replace the lowest-scoring pair with colors from more distinct named color regions.
- Increase lightness or hue separation for the pair with the smallest perceptual distance.
- If two colors would still both be called the same broad name, move one color into a different named region of color space.
