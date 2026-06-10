---
id: use-a-colorblind-safe-color-palette
title: Use a colorblind-safe color palette
bibliography: references.bib
description: For visual reading of charts that encode information with color, use
  a colorblind-safe palette on the chart's color encoding to improve accessibility
  and mitigate indistinguishable color categories for readers with color vision deficiencies.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility:use
- lever:encoding
- aesthetic:color:use
- channel:color-hue:use
- needs:color-vision-deficiency
---

## Revise the color palette <!-- role: advice -->

Test the chart's color palette with a color vision deficiency simulation and keep only colors that remain distinguishable. For example, run the palette through Viz Palette or Chroma and revise any palette that produces major warnings.

## Why palette simulation works <!-- role: reason -->

When chart colors collapse together under a color vision deficiency simulation, the encoded groups stop being visually separable. Testing and revising the palette before release keeps the color categories distinguishable for readers who do not perceive the original hue differences.

**Mechanism:** A simulated CVD check reveals when nominally different chart colors become hard to tell apart, so palette edits can restore visible separation before the chart is published.

**Evidence:** Chartability defines a non-CVD-friendly palette as a perceivable accessibility problem and directs practitioners to test chart palettes with Viz Palette or Chroma, treating major warnings as failures [@elavskyHowAccessibleMy2022]. A heuristic evaluation methodology for charts includes color vision deficiency accessibility, and the cited palette tools explicitly support CVD simulation for chart palette checking [@alcaraz_martinez_methodology_for_2022; @susielu_viz_palette; @vis4_chromajs_colour].

**Notes:** Do not assume that high contrast or added textures remove the need to test the palette itself.

## Use when the chart relies on color differences <!-- role: context -->

- **User Goal:** Distinguish encoded groups, categories, or values by color.
- **Data:** The chart uses multiple color values as an information-carrying encoding.
- **Chart Setting:** The chart already has a chosen palette that can be previewed or edited in a palette checker.
- **Audience:** Readers include people with color vision deficiencies.
- **Success Criterion:** The palette remains distinguishable in a CVD simulation and does not trigger major warnings.

## Do not apply when there is no color encoding to revise <!-- role: exceptions -->

**Break it when:** the chart does not use a color palette to distinguish information. **Why:** there is no color encoding to test or revise for color vision deficiency friendliness.

## Costs of changing the palette <!-- role: costs -->

**Sacrifice:** Some original color choices may need to change.
**Risk:** Treating high contrast or textures as a substitute for palette testing can leave palette-specific CVD failures in place.
**Mitigation:** Re-run the revised palette through a CVD simulator and clear major warnings before finalizing it.

## Common palette-testing failure <!-- role: mistakes -->

**Mistake:** Assume that adding high contrast or textures makes any palette colorblind-safe without testing the palette itself. **Why it fails:** the heuristic explicitly requires checking the color scheme against CVD simulations.

## Check the palette with a simulator <!-- role: check -->

**Failure Sign:** Different encoded colors become hard to distinguish in a CVD preview or the tool reports a major warning.
**Quick Check:** Preview the chart palette in Viz Palette or Chroma with a color vision deficiency simulation.
**Stronger Test:** Treat any major warning from either tool as a failure and revise the palette.

## Fix the failing palette <!-- role: fix -->

- Replace the current palette with one that remains distinguishable in a CVD simulation.
- Edit the palette colors in Viz Palette or Chroma and re-run the simulation after each change.
- Apply the revised palette back to the chart only after the simulation no longer shows major warnings.
