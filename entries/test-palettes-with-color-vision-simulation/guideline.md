---
id: test-palettes-with-color-vision-simulation
title: Test the palette with a color-vision simulator
bibliography: references.bib
description: For charts that rely on color differences, use color-vision simulation
  on the chosen palette to improve accessibility and mitigate undetected color collisions
  for readers with color-vision deficiency.
labels:
- purpose:refine
- basis:heuristic
- quality:accessibility
- lever:encoding
- needs:color-vision-deficiency
- polish:palette
---

## Simulate color-vision deficiencies <!-- role: advice -->

Test the palette with a color-vision simulator before publishing. For example, preview the same colors under different types of colorblindness and revise color pairs that collapse together.

## Why simulation is necessary <!-- role: reason -->

A palette can look distinct to the designer and still fail for readers with color-vision deficiencies. Simulation exposes those collisions before the chart is published.

**Mechanism:** Viewing the palette through color-vision simulations shows whether readers who perceive color differently can still distinguish the encoded differences.

**Evidence:** The post recommends checking whether chosen colors can be distinguished by colorblind people and lists simulators that show how colors appear for different types of colorblindness [@muth_colorguide_2018].

## Use when color differences carry meaning <!-- role: context -->

- **User Goal:** Keep color-coded distinctions readable for more readers.
- **Task:** Validate whether series, categories, or value steps remain separable.
- **Data:** Any data encoded with multiple meaningful colors.
- **Chart Setting:** The chart depends on color differences to communicate distinctions.
- **Audience:** Readers may include people with different types of color-vision deficiency.
- **Success Criterion:** The encoded colors remain distinguishable in simulation.

## Do not use when color is not carrying the distinction <!-- role: exceptions -->

**Break it when:** The chart does not rely on color differences for interpretation. **Why:** There are no meaningful color distinctions to validate.

## Tradeoffs of simulation review <!-- role: costs -->

**Sacrifice:** You add a review step to the palette workflow.\
**Risk:** A palette that looks fine in normal vision may merge in simulated views.\
**Mitigation:** Run the simulation while choosing colors, not only at the end.

## Common misuse of accessible palettes <!-- role: mistakes -->

**Mistake:** Judging the palette only in normal vision. **Why it fails:** It hides color collisions that some readers will experience.

## Check whether colors collapse in simulation <!-- role: check -->

**Failure Sign:** Two or more encoded colors become hard to tell apart in the simulation.\
**Quick Check:** Run the palette through one color-vision simulator.\
**Stronger Test:** Check the palette under multiple simulated types of colorblindness.

## Fix color collisions <!-- role: fix -->

- Replace colors that merge under simulation.
- Increase separation between colors that become similar.
- Re-run the simulator after each palette revision.
