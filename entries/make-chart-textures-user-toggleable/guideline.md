---
id: make-chart-textures-user-toggleable
title: Let users toggle chart textures
bibliography: references.bib
description: For accessible viewing of charts that use texture on fills, use user-controlled
  texture toggles on chart encodings to improve accessibility and mitigate fixed-texture
  visual complexity for audiences with differing visual access needs.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- channel:texture:use
- needs:color-vision-deficiency
---

## Texture toggle <!-- role: advice -->

Add a user control that turns chart textures on or off instead of fixing them in one state. For example, let readers toggle patterned fills on marks or textured colour-scale fills, rather than leaving patterns permanently on by default.

## Why texture toggles help <!-- role: reason -->

Texture controls let readers choose between stronger patterned differentiation and a simpler visual surface. That matters because persistent patterns can help some readers distinguish encodings, but can also add visual complexity for others.

**Mechanism:** A texture toggle gives readers direct control over a noncolor cue. This reduces unnecessary visual complexity for readers who do not want textures while preserving a way to enable patterned differentiation when it helps.

**Evidence:** Chartability states that chart textures used on fills must be able to be turned on or off according to user preference, and it notes that textures left on by default can create accessibility barriers through visual complexity and loss of pre-attentive features [@elavskyHowAccessibleMy2022]. The linked texture experiments show that adjusting texture density and pattern can improve chart accessibility for colour-blind users [@observablehq_experimental_colour].

**Notes:** This guideline addresses conflicting access needs by avoiding a single fixed texture treatment for everyone.

## Use when textures are part of the encoding <!-- role: context -->

- **User Goal:** Read the chart with a preferred balance between redundant differentiation and visual simplicity.
- **Data:** Encodings where texture is applied on fills or layered with colour.
- **Chart Setting:** The chart uses patterned fills, textured colour scales, or other chart textures as part of the presentation.
- **Audience:** Mixed audiences, including readers who benefit from noncolor differentiation and readers who find persistent textures visually complex.
- **Success Criterion:** Readers can switch textures on or off according to preference.

## Do not apply when no textures are present <!-- role: exceptions -->

**Break it when:** The chart does not use textures anywhere in its encoding or presentation. **Why:** There is no texture state for the user to adjust.

## Tradeoffs of texture toggles <!-- role: costs -->

**Sacrifice:** A texture toggle adds another presentation choice to the chart.
**Risk:** Leaving textures fixed in one state can either add unnecessary visual complexity or remove a preferred noncolor cue.
**Mitigation:** Use one explicit on/off control and apply it consistently to all textured fills.

## Common mistake with texture toggles <!-- role: mistakes -->

**Mistake:** Applying textures permanently with no user control. **Why it fails:** Some readers are forced to read through extra visual complexity, while others cannot enable the patterned cue they prefer.

## Check texture control <!-- role: check -->

**Failure Sign:** Patterned fills are always on or always off, with no visible way to change them.
**Quick Check:** Open the chart and look for a control that toggles textures for the textured marks.
**Stronger Test:** Switch the texture setting and confirm that the chart updates its textured fills to match the chosen state.

## Fix fixed textures <!-- role: fix -->

- Add a visible on/off control for chart textures.
- Apply the control to every textured fill used in the chart.
- If textures are on by default, make them removable by the reader.
