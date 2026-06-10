---
id: use-less-saturated-colors-for-racial-categories
title: Use less-saturated colors for racial categories
bibliography: references.bib
description: For non-temporal comparison of racial or regional groups, prefer less-saturated
  category colors on categorical palettes to prevent loaded color connotations and
  mitigate strong red, green, or blue associations for readers of race- or region-focused
  graphics.
labels:
- purpose:refine
- basis:heuristic
- data:categorical
- quality:trust
- lever:encoding
- polish:palette
- aesthetic:color:use
- channel:color-saturation:use
---

## Saturation reduction <!-- role: advice -->

Tone down saturation when color encodes racial or regional categories. For example, replace crayon-like red, green, or dark blue fills with softer versions, and add darker or more saturated outlines when pale fills become hard to distinguish or fail contrast checks.

## Why lower saturation helps <!-- role: reason -->

Highly saturated colors come with strong built-in meanings. Muting them keeps the palette focused on category distinction instead of importing ideas like danger, positivity, competence, or importance.

**Mechanism:** Less-saturated colors weaken default associations attached to vivid red, green, and blue while preserving a full palette for categorical comparison.

**Evidence:** The source recommends toned-down colors for racial categories because saturated colors bring strong associations such as danger, positivity, competence, or royalty, and it notes that darker or more saturated outlines can restore distinction and contrast when pale fills become hard to read [@muth_race_ethnicity_colors_2024].

## When to reduce saturation <!-- role: context -->

- **User Goal:** Use color for category identity without adding loaded meaning.
- **Task:** Compare or explain racial or regional groups.
- **Data:** Categorical groups encoded with different hues.
- **Chart Setting:** A chart or map using a multicolor palette.
- **Audience:** Mixed readers, including readers who may struggle to distinguish pale fills.
- **Success Criterion:** Category colors avoid strong semantic baggage while remaining distinguishable.

## When lower saturation needs support <!-- role: exceptions -->

**Break it when:** the muted fills become hard to distinguish for colorblind readers or bright pastels fail color-contrast accessibility tests. **Why:** the source notes that less-saturated palettes can lose separability and contrast unless supported with darker or more saturated outlines.

## Costs of reducing saturation <!-- role: costs -->

**Sacrifice:** You give up some visual punch.
**Risk:** Pale fills can blur together or fail contrast checks.
**Mitigation:** Keep the toned-down fills but add darker or more saturated outlines.

## Common saturation mistake <!-- role: mistakes -->

**Mistake:** Keeping strong crayon red, green, or dark blue because they look vivid. **Why it fails:** Those colors bring positive, danger, or status meanings into the category encoding.

## How to check saturation choices <!-- role: check -->

**Failure Sign:** One category uses a vivid crayon-like hue or several pale fills blur together.
**Quick Check:** Inspect the palette for strong red, green, or dark blue fills.
**Stronger Test:** Run a contrast check on pale fills and verify that categories remain distinguishable when the outlines are included.

## How to fix saturation choices <!-- role: fix -->

- Reduce saturation on the category fills.
- Shift vivid red, green, or blue slightly away from their strongest canonical hues.
- Add darker or more saturated outlines around pale fills when distinction or contrast drops.
