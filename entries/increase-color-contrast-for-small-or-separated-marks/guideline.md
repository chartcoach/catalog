---
id: increase-color-contrast-for-small-or-separated-marks
title: Increase color contrast for small or separated marks
bibliography: references.bib
description: For comparison in charts with small or widely separated marks, use stronger
  hue or lightness contrast on the colored marks to improve readability and mitigate
  hard-to-distinguish comparisons.
labels:
- purpose:refine
- basis:heuristic
- task:compare
- quality:readability
- lever:encoding
- channel:color-hue:use
- polish:palette
---

## Contrast for small marks <!-- role: advice -->

Increase hue or lightness contrast when the colored marks are small and far apart. For example, give thin lines or small points clearly different colors, but use more toned-down colors only for larger areas that sit next to each other.

## Why mark size and distance change color needs <!-- role: reason -->

Color comparison gets harder when marks are tiny or separated by empty space because the eye cannot compare them as directly.

**Mechanism:** Stronger hue or brightness differences help readers distinguish small lines and points across distance, while large adjacent areas can be compared with less contrast.

**Evidence:** The post says that smaller areas and bigger distances make color comparison harder, recommends high contrast in hue or brightness for small points or lines, and notes that big areas can handle toned-down colors with little contrast when no background color sits between them [@muth_colors_2018].

## When to increase contrast <!-- role: context -->

- **User Goal:** Compare colored marks accurately.
- **Chart Setting:** Marks are thin, small, or far apart.
- **Data:** Color distinguishes multiple series, groups, or observations.
- **Success Criterion:** Readers can tell the colored marks apart quickly.

## When lower contrast is acceptable <!-- role: exceptions -->

**Break it when:** The colored areas are large and adjacent, especially with no background color between them. **Why:** The post says those situations can work with more toned-down colors.

## Tradeoffs of stronger mark contrast <!-- role: costs -->

**Sacrifice:** The palette may look less subtle.
**Risk:** Over-contrasted colors can make the chart feel busy.
**Mitigation:** Reserve the strongest contrast for small or distant marks only.

## Common mark-contrast mistake <!-- role: mistakes -->

**Mistake:** Applying a low-contrast palette to thin lines or small points that are far apart. **Why it fails:** Readers struggle to distinguish the marks and compare them reliably.

## How to check mark contrast <!-- role: check -->

**Failure Sign:** Small colored marks look too similar to tell apart at normal chart size.
**Quick Check:** Compare the most similar-colored small marks without zooming in.
**Stronger Test:** Check whether the same colors would still be distinguishable if the marks were viewed at typical article or dashboard size.

## How to fix weak mark contrast <!-- role: fix -->

- Increase hue contrast between small colored marks.
- Increase lightness contrast between small colored marks.
- Tone colors down only on larger adjacent areas that can tolerate lower contrast.
