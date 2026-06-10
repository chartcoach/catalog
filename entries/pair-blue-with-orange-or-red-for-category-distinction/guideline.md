---
id: pair-blue-with-orange-or-red-for-category-distinction
title: Pair blue with orange or red when hue must distinguish categories
bibliography: references.bib
description: For few-category comparisons, prefer blue paired with orange or red on
  color-encoded marks to improve distinguishability and mitigate confusing same-lightness
  hue pairings for readers with color-vision deficiency.
labels:
- purpose:refine
- basis:heuristic
- quality:accessibility
- lever:encoding
- group-cardinality:few
- channel:color-hue:use
- needs:color-vision-deficiency
- polish:palette
---

## Pair safe hues <!-- role: advice -->

Use blue with orange or red when category identity depends on hue. For example, replace green–orange, green–red, or same-lightness green–blue pairings with a blue–orange or blue–red pair in a two-category chart or map.

## Why this hue pair works <!-- role: reason -->

Blue stays closest to how readers with and without common red-green color-vision deficiencies perceive color, so it is the most stable anchor hue. Orange or red stays more separable from blue than nearby hues such as purple, which can collapse into a confusingly similar pair.

**Mechanism:** Stable hue separation lets readers tell categories apart without depending on fine color discrimination.

**Evidence:** Blue is identified as the safest hue, blue paired with orange or red is recommended as a safe choice across common color-vision deficiencies, and nearby pairs such as blue and purple are described as especially hard to distinguish. [@muth_colorblindness_2020]

## Use when hue carries category identity <!-- role: context -->

- **User Goal:** Distinguish a small number of categories quickly.
- **Task:** Category lookup or comparison by color.
- **Data:** A few discrete groups encoded primarily by hue.
- **Chart Setting:** A chart or map where color is doing most of the grouping work.
- **Audience:** Readers who may include people with color-vision deficiency.
- **Success Criterion:** The groups still look distinct without relying on subtle hue differences.

## Do not rely on this pair as the only solution <!-- role: exceptions -->

**Break it when:** The colors can already be separated clearly by lightness. **Why:** The article states that any hues can work when their lightness is distinct, so hue choice is no longer the deciding lever.

## Costs of safer hue pairing <!-- role: costs -->

**Sacrifice:** You give up tighter, nearby-hue palettes.
**Risk:** The palette can feel less visually cohesive if you were aiming for adjacent hues such as blue and purple.
**Mitigation:** Adjust the exact blue or orange/red within the same hue family instead of moving to a nearby confusing hue.

## Common hue-pair failure <!-- role: mistakes -->

**Mistake:** Using green with orange/red, or using green with blue at the same lightness, when hue is the only separator. **Why it fails:** Those pairs are explicitly called out as hard for colorblind readers to tell apart.

## How to verify the pair <!-- role: check -->

**Failure Sign:** The two categories collapse into nearly the same color in a colorblind simulation.
**Quick Check:** Simulate red-blind and green-blind vision and inspect whether the pair still separates cleanly.
**Stronger Test:** Ask a colorblind reader whether they can identify each category without extra help.

## What to change <!-- role: fix -->

- Replace a green-based category color with blue.
- Pair the blue with orange or red instead of a nearby hue such as purple.
- If you must keep the current hues, separate them more strongly by lightness.
