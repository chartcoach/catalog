---
id: avoid-thin-font-weights-in-chart-text
title: Avoid thin font weights in chart text
bibliography: references.bib
description: For labels, annotations, and titles in charts, avoid thin font weights
  on chart text to improve readability and mitigate faint-looking small text for readers
  viewing web visualizations.
labels:
- purpose:refine
- basis:heuristic
- quality:readability
- lever:text-annotation
- aesthetic:style:avoid
- access:contrast:use
---

## Replace thin weights in small chart text <!-- role: advice -->

Do not use thin or light weights for small chart text. For example, keep labels, notes, and annotations in regular or medium weight, and reserve thin weights for large high-contrast titles if you use them at all.

## Why avoiding thin weights works <!-- role: reason -->

Thin strokes make text look visually lighter even when the color is dark. That weakens readability fast in small labels and notes.

**Mechanism:** Thinner strokes reduce the apparent darkness of text, so small chart text starts to look faint and becomes harder to read.

**Evidence:** The article warns that thin and light weights look as if they are set in a brighter color and are really hard to read, recommending them only in high-contrast color and large sizes, often for titles only [@muth_fonts_2022].

## When to avoid thin weights <!-- role: context -->

- **User Goal:** Keep text readable while showing hierarchy.
- **Chart Setting:** Labels, notes, annotations, or other small chart text appear on screen.
- **Audience:** Readers are viewing the chart at normal reading size.
- **Success Criterion:** Secondary text is still clearly legible.

## When to break the thin-weight rule <!-- role: exceptions -->

**Break it when:** The text is large, high-contrast, and used as a title. **Why:** Thin weights are only workable when size and contrast compensate for their delicate strokes.

## Tradeoffs of avoiding thin weights <!-- role: costs -->

**Sacrifice:** You give up some delicate or airy typographic styling.
**Risk:** Using thin weight to make text feel less important still leaves it really hard to read.
**Mitigation:** Keep small text in regular or medium weight and reserve thin weight for large titles only.

## Common thin-weight mistake <!-- role: mistakes -->

**Mistake:** Using a thin or light weight to make small text seem less important. **Why it fails:** The text starts to look faint, as if it were gray, and becomes hard to read.

## How to check thin weights <!-- role: check -->

**Failure Sign:** Dark text still looks washed out or faint.
**Quick Check:** Inspect the font weight used on labels, notes, and annotations and flag thin or light settings.
**Stronger Test:** Compare the same text in regular weight and keep the version that is easier to read.

## How to fix thin weights <!-- role: fix -->

- Change thin or light small text to regular or medium weight.
- Increase contrast if any thin text must remain.
- Restrict thin weights to large titles only.
