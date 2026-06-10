---
id: avoid-red-and-green-pairs-with-similar-brightness
title: Avoid red and green pairs with similar brightness
bibliography: references.bib
description: For categorical palette design intended for broad readership, avoid red
  and green category colors with similar brightness on data marks to improve accessibility
  and mitigate category confusion for readers with color vision deficiency.
labels:
- purpose:refine
- basis:heuristic
- data:categorical
- quality:accessibility
- lever:encoding
- needs:color-vision-deficiency
- polish:palette
- aesthetic:color:avoid
---

## Separate risky red-green pairs <!-- role: advice -->

Do not use red and green with similar brightness as the main distinction between categories. For example, change one hue or increase the brightness difference, then run a colorblind check before finalizing the palette.

## Why this pair is risky <!-- role: reason -->

A red-green pair can look distinct to some readers and collapse for others. Similar brightness makes that problem harder to recover from.

**Mechanism:** When hue and brightness are both too similar, readers with color vision deficiency have fewer cues left to separate the categories.

**Evidence:** The article says final palette colors should be distinct for colorblind people too and specifically warns against choosing red and green with similar brightness [@muth_good_color_palettes_2024].

## Use when red and green are candidate category colors <!-- role: context -->

- **User Goal:** Differentiate categories accessibly.
- **Data:** Categorical groups.
- **Chart Setting:** The palette currently uses red and green for different categories.
- **Audience:** Readers include people with color vision deficiency.
- **Success Criterion:** The categories remain distinct under a colorblind check.

## Do not use when brightness already separates the pair <!-- role: exceptions -->

**Break it when:** The red and green are clearly separated by brightness. **Why:** The article flags similar brightness as the risky condition.

## Tradeoffs of changing the pair <!-- role: costs -->

**Sacrifice:** You may lose a familiar red-versus-green convention.
**Risk:** Changing one color can weaken an association the chart intentionally wanted.
**Mitigation:** Keep the needed meaning, but spread the pair farther apart in hue or brightness.

## Common red-green mistake <!-- role: mistakes -->

**Mistake:** Keep a similar-brightness red-green pair because it looks distinct enough to noncolorblind reviewers. **Why it fails:** The pair can still collapse for readers with color vision deficiency.

## Check red-green accessibility <!-- role: check -->

**Failure Sign:** The two categories become hard to tell apart in a colorblind view.
**Quick Check:** Run a colorblindness simulator or built-in colorblind check on the palette.
**Stronger Test:** Review the actual chart with the simulated view and confirm that the categories still separate cleanly.

## Fix a risky red-green pair <!-- role: fix -->

- Replace one of the two hues so the pair is no longer red versus green.
- Increase the brightness difference between the two colors.
- Rerun the colorblind check after each change.
