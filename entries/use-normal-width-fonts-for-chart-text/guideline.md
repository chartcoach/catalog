---
id: use-normal-width-fonts-for-chart-text
title: Use normal-width fonts for chart text
bibliography: references.bib
description: For labels and numbers under space constraints in charts, prefer normal-width
  typefaces on chart text to improve readability and mitigate cramped text from condensed
  fonts for readers scanning values.
labels:
- purpose:refine
- basis:heuristic
- quality:readability
- lever:text-annotation
- aesthetic:style:use
---

## Swap condensed chart text for normal-width text <!-- role: advice -->

Use a normal-width typeface for chart labels and numbers, even when space is tight. For example, replace a condensed label font with a slightly smaller normal-width font, and keep very narrow or very wide styles for large display titles rather than dense labels.

## Why normal-width text works <!-- role: reason -->

Condensed letters save space, but they also make characters harder to decipher. A slightly smaller normal-width font often preserves readability better than a larger condensed one.

**Mechanism:** Normal-width letterforms keep enough horizontal space for characters to stay distinct, which makes dense chart text easier to read.

**Evidence:** The article says narrow fonts are harder to read than normal-width fonts, notes that very wide fonts use too much space, and states that normal-width text in a smaller size is often as or more readable than larger text in a narrow face [@muth_fonts_2022].

## When to use normal-width text <!-- role: context -->

- **User Goal:** Fit labels or numbers into limited space without hurting readability.
- **Chart Setting:** A chart uses many short labels or values in a constrained layout.
- **Audience:** Readers must decipher labels quickly.
- **Success Criterion:** Text remains readable without looking cramped.

## When to break the normal-width rule <!-- role: exceptions -->

**Break it when:** The text is very large, such as a display title. **Why:** Extremely narrow or wide styles can work more successfully at large sizes than in dense chart labels.

## Tradeoffs of normal-width text <!-- role: costs -->

**Sacrifice:** You give up some of the space savings of condensed typography.
**Risk:** Keeping a large size by switching to a narrow face can make the design feel cramped.
**Mitigation:** Reduce font size slightly before you reduce character width.

## Common normal-width text mistake <!-- role: mistakes -->

**Mistake:** Preserving a larger font size by switching labels to a condensed face. **Why it fails:** Compressed characters are harder to decipher than a slightly smaller normal-width alternative.

## How to check normal-width text <!-- role: check -->

**Failure Sign:** Labels look cramped, squeezed, or overly narrow.
**Quick Check:** Compare the current condensed text with a slightly smaller normal-width version.
**Stronger Test:** Keep the version that is easier to decipher at the intended reading size.

## How to fix normal-width text <!-- role: fix -->

- Replace condensed label text with the normal-width cut of the typeface.
- Lower font size before switching to a narrow width.
- Reserve very narrow or very wide styles for large title text only.
