---
id: adjust-uppercase-with-spacing-size-and-weight
title: Adjust uppercase text with more spacing, smaller size, and bolder weight
bibliography: references.bib
description: For short labels and headings that must be set in uppercase, use extra
  letter spacing with smaller, slightly bolder uppercase text on chart labels to improve
  readability and mitigate overly wide, dense all-caps text for readers scanning interface-like
  elements.
labels:
- purpose:refine
- basis:heuristic
- quality:readability
- lever:text-annotation
- polish:spacing
---

## Tune spacing, size, and weight after uppercasing <!-- role: advice -->

When you convert chart text to uppercase, increase letter spacing, reduce the font size, and then make the text slightly bolder. For example, use this sequence on short axis labels, map region labels, or table headers so the all-caps version stays closer in length and stroke weight to the original sentence-case text.

## Why uppercase tuning works <!-- role: reason -->

Uppercasing text changes more than the case. The text becomes wider and denser, so it needs compensating adjustments to keep its size and texture under control.

**Mechanism:** More letter spacing opens up dense uppercase text, a smaller size offsets the added width, and slightly more weight restores the stroke presence lost when the size is reduced.

**Evidence:** The article demonstrates that uppercase text becomes wider and denser than sentence case, then recommends three specific adjustments—more letter spacing, smaller size, and bolder weight—to bring the uppercase version closer to the original text's length and stroke width [@muth_fonts_2022].

## When to tune uppercase text <!-- role: context -->

- **User Goal:** Keep uppercase labels tidy without making them too long or dense.
- **Chart Setting:** A short label or heading has already been chosen for uppercase styling.
- **Audience:** Readers are scanning short labels rather than reading prose.
- **Success Criterion:** The uppercase version stays compact and legible.

## When to break the uppercase tuning rule <!-- role: exceptions -->

**Break it when:** The text stays in sentence case. **Why:** These adjustments are needed after converting text to uppercase, not before.

## Tradeoffs of uppercase tuning <!-- role: costs -->

**Sacrifice:** You add manual tuning work to the typography.
**Risk:** Uppercasing without these adjustments makes text longer and denser than surrounding labels.
**Mitigation:** Apply the three adjustments in sequence until the uppercase text feels closer to the original sentence-case version.

## Common uppercase tuning mistake <!-- role: mistakes -->

**Mistake:** Capitalizing text and leaving spacing, size, and weight unchanged. **Why it fails:** The uppercase label expands and looks too dense compared with surrounding text.

## How to check uppercase tuning <!-- role: check -->

**Failure Sign:** The uppercase label is much longer or denser than the sentence-case version.
**Quick Check:** Compare the sentence-case and uppercase versions side by side.
**Stronger Test:** Tune letter spacing, size, and weight until the uppercase version is closer to the original length and stroke weight.

## How to fix uppercase tuning <!-- role: fix -->

- Increase letter spacing after capitalizing the text.
- Reduce the font size to shorten the uppercase label.
- Make the uppercase text slightly bolder to restore stroke weight.
