---
id: check-text-contrast-on-colored-backgrounds
title: Check text contrast before placing text on colored backgrounds
bibliography: references.bib
description: For labels or annotations placed on colored areas, use a contrast check
  on text and background colors to improve accessibility and mitigate unreadable text
  for viewers reading labels on color fills.
labels:
- purpose:refine
- basis:heuristic
- quality:accessibility
- lever:encoding
- component:label:use
- access:contrast:use
---

## Verify text-background contrast <!-- role: advice -->

Check text color against its background before placing text on a colored mark. For example, test labels placed on map fills or other colored areas, and reject combinations such as red and blue when they do not pass the contrast review.

## Why contrast checking matters <!-- role: reason -->

A color pairing can look appealing and still be unreadable when used for chart text. A contrast check turns that into a concrete pass-or-fail decision tied to text size.

**Mechanism:** Contrast testing shows whether text remains readable on a colored background and whether the pairing only works at larger sizes.

**Evidence:** The post recommends checking contrast when placing text on colors and notes that a contrast tool reports readability by text size, giving red and blue as an example that does not pass [@muth_colorguide_2018].

## Use when text sits on color fills <!-- role: context -->

- **User Goal:** Keep labels and annotations readable on colored marks.
- **Task:** Validate text readability against the chosen fill color.
- **Data:** Any chart where text is placed directly on colored areas.
- **Chart Setting:** Maps or other charts with labels or annotations inside colored regions.
- **Audience:** Readers need to read text directly on top of the encoded color.
- **Success Criterion:** The text-background pair passes for the intended text size.

## Do not use when text is not placed on colored areas <!-- role: exceptions -->

**Break it when:** The chart does not place text on colored backgrounds. **Why:** This check is specifically about text sitting on top of color.

## Tradeoffs of contrast checking <!-- role: costs -->

**Sacrifice:** You may give up some preferred color pairings.\
**Risk:** Decorative combinations can fail once used for actual chart text.\
**Mitigation:** Choose the text or background color based on the contrast result and intended text size.

## Common misuse of text on color <!-- role: mistakes -->

**Mistake:** Choosing text and background colors by aesthetic match alone. **Why it fails:** Some pairs are not readable at the sizes used in charts.

## Check whether the pair passes <!-- role: check -->

**Failure Sign:** The label is hard to read on the colored area.\
**Quick Check:** Run the text and background pair through a contrast checker.\
**Stronger Test:** Confirm that the pair passes for the actual text size you plan to use.

## Fix low-contrast text <!-- role: fix -->

- Change the text color to one that passes on the existing background.
- Change the background color behind the text.
- Increase text size only if the contrast check shows the pair becomes readable at that size.
