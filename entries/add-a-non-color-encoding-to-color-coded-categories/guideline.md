---
id: add-a-non-color-encoding-to-color-coded-categories
title: Add a non-color encoding to color-coded categories
bibliography: references.bib
description: For categorical interpretation, use redundant non-color encoding on color-coded
  marks to improve accessibility and mitigate meaning loss from hue-only distinctions
  for readers with color-vision deficiencies.
labels:
- purpose:refine
- basis:accessibility
- data:categorical
- quality:accessibility
- lever:encoding
- needs:color-vision-deficiency
- access:noncolor:use
---

## Add a redundant non-color encoding <!-- role: advice -->

Pair every meaningful color distinction with a second visual channel. For example, add textures, shape differences, or size differences to filled categorical marks, and use distinct dash patterns to distinguish lines and paths.

## Why redundant encoding works <!-- role: reason -->

A second visual cue keeps category meaning available when hue differences are missed, collapsed, or hard to distinguish. Readers can still separate groups because the chart does not depend on color alone to carry the distinction.

**Mechanism:** Redundant encoding moves category identification from a single fragile cue to multiple visible cues, so the same meaning survives when color perception varies.

**Evidence:** Chartability states that meaningful information must not be communicated by color alone and, for categorical color schemes, requires a second channel such as texture, shape, size, or dash patterns [@elavskyHowAccessibleMy2022]. WCAG's understanding guidance also requires an additional cue beyond colour, and the linked visualization examples show category distinctions made accessible by adding patterns or shapes [@w3c_understanding_use; @observablehq_no_use].

**Notes:** The source explicitly limits this guidance to categorical color schemes and notes that effective strategies for numerical color scales need more research.

## Use when color carries category identity <!-- role: context -->

- **User Goal:** Identify which marks belong to which category or status.
- **Task:** Distinguish groups that are currently encoded by color.
- **Data:** Categorical groups or classes.
- **Chart Setting:** A chart uses color on filled elements, lines, or paths to convey meaningful or essential information.
- **Audience:** Readers may include people with color-vision deficiencies.
- **Success Criterion:** The category distinction remains readable without relying on hue alone.

## Do not extend this rule to unsupported color scales <!-- role: exceptions -->

**Break it when:** Color encodes a numerical progression such as a sequential or ordinal scale rather than categories. **Why:** The provided source notes that effective non-color strategies for these scales are still underexplored, so this specific repair is not directly supported there.

## Tradeoffs of redundant category encoding <!-- role: costs -->

**Sacrifice:** You give up a color-only encoding.
**Risk:** This repair can be difficult to apply cleanly in data visualization, especially if you try to carry it into numerically scaled color schemes.
**Mitigation:** Keep this guideline focused on categorical color schemes and add one non-color cue that matches the mark type.

## Common failure with color-coded categories <!-- role: mistakes -->

**Mistake:** Use color as the only way to tell categories apart. **Why it fails:** Essential meaning disappears for readers who cannot reliably distinguish the hue differences.

## Check whether color is carrying meaning alone <!-- role: check -->

**Failure Sign:** Two categories differ only by color, with no texture, shape, size, or line-style difference.
**Quick Check:** Ask whether the category meaning would still be readable if hue differences were unavailable. If not, the chart fails this guideline.
**Stronger Test:** Inspect each color-coded mark type and confirm that filled elements also vary by texture, shape, or size, or that lines and paths also vary by dash pattern.

## Fix the encoding <!-- role: fix -->

- Add a texture to filled categorical marks that are currently separated only by color.
- Add shape or size differences to filled categorical marks when texture is not enough or not available.
- Apply distinct dash patterns to lines or paths that currently differ only by color.
- Rework the category encoding until every meaningful distinction can be read without relying on color alone.
