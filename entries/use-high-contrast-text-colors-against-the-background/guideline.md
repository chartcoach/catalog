---
id: use-high-contrast-text-colors-against-the-background
title: Use high-contrast text colors against the background
bibliography: references.bib
description: For chart text on screens, use high-contrast foreground and background
  colors to improve accessibility and mitigate unreadable labels in low-light viewing.
labels:
- purpose:refine
- basis:heuristic
- quality:accessibility
- lever:encoding
- access:contrast:use
- channel:color-lightness:use
- aesthetic:color:use
---

## Text contrast <!-- role: advice -->

Give chart text strong contrast against its background. For example, keep the contrast ratio at least 2.5 for big text and at least 4 for small text, and avoid complementary hue pairs or bright background colors behind the text.

## Why high text contrast matters <!-- role: reason -->

Text is the first chart element to fail when contrast is weak, especially on screens and in poor viewing conditions.

**Mechanism:** Higher contrast makes labels and annotations readable at smaller sizes and under less favorable lighting.

**Evidence:** The post says readers should be able to read charts on their screens even in low light, notes that this is especially important for text, gives minimum contrast ratios of 2.5 for big text and 4 for small text, and warns against complementary hues and bright backgrounds [@muth_colors_2018].

## When to check text contrast <!-- role: context -->

- **User Goal:** Read chart text comfortably on screen.
- **Chart Setting:** Text sits on colored or light backgrounds.
- **Data:** Labels, annotations, and other text are necessary to interpret the chart.
- **Success Criterion:** Text remains readable without straining, including small text.

## When to use the lower threshold <!-- role: exceptions -->

**Break it when:** The text is large. **Why:** The post sets a lower minimum contrast ratio for big text than for small text.

## Tradeoffs of stronger contrast <!-- role: costs -->

**Sacrifice:** Softer or more decorative text colors may need to be dropped.
**Risk:** Strong contrast can feel visually harsh if applied without restraint.
**Mitigation:** Keep backgrounds subdued rather than bright, so contrast stays high without adding glare.

## Common text-contrast mistake <!-- role: mistakes -->

**Mistake:** Using low-contrast text or placing text on complementary or bright background colors. **Why it fails:** The text becomes harder to read, especially when it is small.

## How to check text contrast <!-- role: check -->

**Failure Sign:** Small labels look faint against the background.
**Quick Check:** Test the foreground and background pair with a color-contrast tool.
**Stronger Test:** Verify that big text reaches at least 2.5 contrast and small text reaches at least 4.

## How to fix weak text contrast <!-- role: fix -->

- Darken the text color against a light background.
- Lighten or mute the background behind the text.
- Replace complementary foreground-background color pairs.
- Remove bright background colors behind labels and annotations.
