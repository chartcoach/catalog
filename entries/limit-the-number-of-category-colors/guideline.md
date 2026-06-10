---
id: limit-the-number-of-category-colors
title: Limit the number of category colors
bibliography: references.bib
description: For color-coded charts with many groups, avoid large hue counts on encoded
  marks to improve accessibility and mitigate reader dropout for people with color-vision
  deficiency.
labels:
- purpose:refine
- basis:heuristic
- quality:accessibility
- lever:encoding
- group-cardinality:many
- needs:color-vision-deficiency
- polish:focus
---

## Reduce hue count and emphasize only what matters <!-- role: advice -->

Use fewer category colors when many groups would otherwise compete for attention. For example, keep color on only the one or two most important values, tone down the others, or group less important categories instead of assigning every group its own strong hue.

## Why fewer colors help <!-- role: reason -->

Each additional hue raises the chance that some readers will stop trying to decode the chart. A smaller set of emphasized colors makes the intended takeaway easier to see and reduces dependence on subtle color differences.

**Mechanism:** Lower hue count reduces decoding load and makes the most important categories stand out before readers have to interpret the full palette.

**Evidence:** The article states that the more colors are used, the harder they become to tell apart, quotes a colorblind reader who tends to tune out when charts use more than three or four colors without other indicators, and recommends coloring only the most important values while toning down or grouping the rest. [@muth_colorblindness_2020]

## Use when many groups are color-coded <!-- role: context -->

- **User Goal:** Keep a multi-group chart scannable.
- **Task:** Overview and comparison of a chart with many categories.
- **Data:** Many discrete groups that could each receive a different color.
- **Chart Setting:** A chart where color is carrying group identity.
- **Audience:** Readers who may include people with color-vision deficiency.
- **Success Criterion:** The main takeaway is visible without decoding a long palette.

## When this limit matters less <!-- role: exceptions -->

**Break it when:** Other visual indicators such as annotations already identify the groups clearly. **Why:** The article notes that many colors are especially problematic when other indicators are not being used.

## Costs of reducing colors <!-- role: costs -->

**Sacrifice:** You give up one-to-one color coding for every group.
**Risk:** Less important categories may feel visually de-emphasized.
**Mitigation:** Group muted categories or label the important ones directly so the emphasis is intentional.

## Common many-color failure <!-- role: mistakes -->

**Mistake:** Assigning a distinct strong color to every category in a chart with more than a few groups. **Why it fails:** Readers must decode too many hues, and colorblind readers are more likely to give up.

## How to verify the palette size <!-- role: check -->

**Failure Sign:** The chart needs more than three or four strong category colors and still lacks clear noncolor guidance.
**Quick Check:** Count the distinct saturated category colors in use.
**Stronger Test:** Ask whether a reader can identify the one or two key insights before decoding the full palette.

## What to change <!-- role: fix -->

- Keep strong color only on the one or two categories that carry the main message.
- Tone down the remaining categories instead of giving each one a strong distinct hue.
- Group minor categories so fewer distinct colors are needed.
- If many separate groups must remain visible, redesign toward a form that relies less on color and labels data more directly.
