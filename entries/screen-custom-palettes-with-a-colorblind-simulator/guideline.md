---
id: screen-custom-palettes-with-a-colorblind-simulator
title: Screen custom palettes with a colorblind simulator
bibliography: references.bib
description: For custom color encoding, use colorblind simulation on chart images
  or screens to improve accessibility and mitigate unnoticed color collisions for
  readers with color-vision deficiency.
labels:
- purpose:refine
- basis:heuristic
- quality:accessibility
- lever:encoding
- communication:workflow
- needs:color-vision-deficiency
- polish:palette
---

## Test the color encoding before publishing <!-- role: advice -->

Run a colorblind simulation on the chart before publishing when you choose your own colors. For example, inspect a screenshot or the live screen under simulations of the major color-vision deficiencies and look for categories that collapse into the same appearance.

## Why simulation helps <!-- role: reason -->

Simulation can expose color collisions that are easy to miss during design. It is a fast screening step that shows whether the palette survives different kinds of color-vision loss.

**Mechanism:** A simulated view lets the designer see whether the current color encoding still separates marks under different color-vision conditions.

**Evidence:** The article recommends testing chosen colors with colorblind simulators, lists several ways to simulate all three types of colorblindness, and cautions that these previews are only approximate rather than a bulletproof final answer. [@muth_colorblindness_2020]

## Use when you choose or modify colors yourself <!-- role: context -->

- **User Goal:** Catch inaccessible color choices before release.
- **Task:** Palette review and chart QA.
- **Data:** Any visualization where color is doing identification work.
- **Chart Setting:** A chart image or live screen that can be simulated.
- **Audience:** Readers who may include people with color-vision deficiency.
- **Success Criterion:** Hard-to-distinguish colors are found before publication.

## What simulation cannot prove <!-- role: exceptions -->

**Break it when:** You treat the simulation as final proof that the chart is accessible. **Why:** The article says the previews are not 100% correct and that everyone is different.

## Costs of simulator screening <!-- role: costs -->

**Sacrifice:** You add an extra review step to the workflow.
**Risk:** Simulation can create false confidence if you stop there.
**Mitigation:** Add a second visual variable or ask colorblind people to review the chart as well.

## Common testing failure <!-- role: mistakes -->

**Mistake:** Skipping simulation entirely, or relying on simulation alone without any noncolor encoding. **Why it fails:** The first leaves color collisions undiscovered, and the second ignores the article's warning that simulation is only approximate.

## How to verify the screening step <!-- role: check -->

**Failure Sign:** You have not viewed the chart under simulated color-vision deficiencies.
**Quick Check:** Run at least one simulation on the chart image or live screen and inspect whether categories remain distinct.
**Stronger Test:** Simulate all three major colorblindness types and then confirm the design with a second encoding or reviewer feedback.

## What to change <!-- role: fix -->

- Run a colorblind simulator on the current chart image or screen.
- Replace or separate any colors that collapse under simulation.
- Add position, shape, pattern, or line style if color alone remains ambiguous.
- Ask a colorblind reader to review the revised chart before finalizing it.
