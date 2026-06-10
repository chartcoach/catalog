---
id: increase-contrast-for-category-colored-annotation-text
title: Increase contrast for category-colored annotation text
bibliography: references.bib
description: For annotations that reuse bright category colors, use higher-contrast
  text styling on colored words to improve readability and mitigate illegible thin
  letterforms for readers reading colored annotation text.
labels:
- purpose:refine
- basis:heuristic
- quality:readability:use
- lever:text-annotation
- component:annotation:use
- access:contrast:use
- aesthetic:color:use
---

## Annotation text contrast <!-- role: advice -->

Adjust annotation styling when a category color works on marks but fails on thin letters. For example, make the annotation text a slightly darker version of the category color or put the color behind the text as a background highlight.

## Why higher-contrast annotation text works <!-- role: reason -->

A color that reads well on a thick bar or line can become hard to read when it is used on small letterforms. Slightly darker text or a colored background preserves the category cue while keeping the annotation legible.

**Mechanism:** Increasing text-background contrast keeps the category reminder visible without losing readability at annotation size.

**Evidence:** The article notes that bright colors that work on bars can become illegible as thin letters, and recommends either darkening the text color a bit or using the category color as a text background instead [@muth_remind_colors_2023].

## When to use higher-contrast annotation text <!-- role: context -->

- **User Goal:** Reuse category colors in annotation text.
- **Data:** Some category colors are bright or light.
- **Chart Setting:** Colored annotation text or text highlights sit on a plain background.
- **Success Criterion:** Every colored word remains easy to read at its displayed size.

## When not to add extra contrast treatment <!-- role: exceptions -->

**Break it when:** The category color already has high contrast as text against the background. **Why:** Extra darkening or background treatment is unnecessary.

## Costs of higher-contrast annotation text <!-- role: costs -->

**Sacrifice:** The text color may no longer match the mark color exactly.
**Risk:** A full background highlight takes more visual space than plain text.
**Mitigation:** Darken the text only a little or highlight only the relevant word or phrase.

## Common contrast mistake <!-- role: mistakes -->

**Mistake:** Reusing a bright bar or line color unchanged in small annotation text. **Why it fails:** The letters become hard to read even though the same color works on the mark itself.

## How to test annotation text contrast <!-- role: check -->

**Failure Sign:** The colored word is noticeably harder to read than nearby dark text.
**Quick Check:** Review the brightest category colors at displayed annotation size and confirm that each colored word is legible.
**Stronger Test:** Compare the colored word against the same background after slight darkening and keep the version that reads clearly.

## How to fix low-contrast annotation text <!-- role: fix -->

- Darken the annotation text to a slightly deeper version of the category color.
- Replace colored text with a background highlight behind the relevant word or phrase.
- Keep the highlight limited to the category term instead of styling the whole sentence.
