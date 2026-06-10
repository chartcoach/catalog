---
id: avoid-brown-and-olive-hues-for-racial-categories
title: Avoid brown and olive hues for racial categories
bibliography: references.bib
description: For non-temporal comparison of racial or ethnic groups, avoid brown and
  olive category colors on categorical palettes to prevent unwanted skin-tone reminders
  and mitigate dislike of the encoded groups for readers of people-focused graphics.
labels:
- purpose:refine
- basis:heuristic
- data:categorical
- quality:trust
- lever:encoding
- polish:palette
- aesthetic:color:avoid
- channel:color-hue:avoid
---

## Brown and olive avoidance <!-- role: advice -->

Avoid brown and olive when a color represents a racial or ethnic group. For example, replace brown or olive bars, series, map fills, or legend swatches with hues that do not echo skin tones.

## Why brown and olive are risky here <!-- role: reason -->

These hues can read as skin-tone proxies even when they are not literal stereotype matches. They also carry a likability penalty that can transfer to how the encoded group feels in the chart.

**Mechanism:** Brown and olive can remind readers of skin tones and can make represented groups feel less favorably treated than groups assigned other colors.

**Evidence:** The source advises avoiding certain shades of brown and olive for racial data because they can be remindful of skin tones and because people tend to like them less than other colors in general [@muth_race_ethnicity_colors_2024].

## When to avoid brown and olive <!-- role: context -->

- **User Goal:** Show racial or ethnic categories respectfully.
- **Task:** Compare or explain differences between categories.
- **Data:** Categorical groups about people.
- **Chart Setting:** A chart or map with one color assigned to each group.
- **Audience:** Mixed readers, including people represented by the data.
- **Success Criterion:** No category color feels like an unwanted skin-tone cue or an unlikeable color assignment.

## When this rule does not apply <!-- role: exceptions -->

**Break it when:** the brown or olive hue is not being used to encode a racial or ethnic category. **Why:** the source’s concern here is specifically how these hues read when they are attached to groups of people.

## Costs of removing brown and olive <!-- role: costs -->

**Sacrifice:** You lose some earthy palette options.
**Risk:** A replacement hue can still introduce another unwanted association if chosen casually.
**Mitigation:** Replace brown or olive with a different non-skin-tone hue rather than with another near-skin-tone substitute.

## Common brown and olive mistake <!-- role: mistakes -->

**Mistake:** Using brown or olive as a “safe” substitute after removing more obvious stereotype colors. **Why it fails:** The category can still read as skin-tone-coded and may feel less liked than categories shown in other hues.

## How to check for brown and olive problems <!-- role: check -->

**Failure Sign:** A racial or ethnic category is shown in brown or olive.
**Quick Check:** Inspect the legend and identify any brown or olive swatches attached to people categories.
**Stronger Test:** Ask whether the hue reminds reviewers of skin tone or feels less pleasant than the rest of the palette.

## How to fix brown and olive problems <!-- role: fix -->

- Replace brown with a different non-skin-tone hue.
- Replace olive with a different non-skin-tone hue.
- Recheck the full palette so no remaining category color still resembles a skin tone.
