---
id: prefer-3d-volume-over-3d-surface-rendering
title: Choose solid 3-D volume rendering instead of floating 3-D surface rendering
bibliography: references.bib
description: For 3-D rendering of 2-D quantitative data, prefer volume-style 3-D rendering
  on line or bar charts to improve aesthetics and mitigate low-preference floating-surface
  forms for viewers judging chart appropriateness.
labels:
- purpose:refine
- basis:empirical
- lever:encoding
- communication:resonance
- quality:aesthetics
- aesthetic:style:use
---

## Use solid 3-D forms when you add depth <!-- role: advice -->

Choose a solid 3-D volume rendering instead of a floating 3-D surface rendering when you decide to add depth. For example, use a filled-under-the-curve 3-D volume line or a full 3-D bar rather than a suspended surface line or top-only surface bar.

## Why solid volumes win within 3-D styles <!-- role: reason -->

Not all 3-D treatments are read the same way. Solid volumes look more like real objects than floating surfaces do.

**Mechanism:** A volume rendering gives the chart a more object-like form, which better matches the paper's preferred kind of 3-D display.

**Evidence:** When the paper compared 3-D types, participants preferred renderings that strongly suggested a solid volume over renderings that looked like surfaces floating in space [@levyGratuitousGraphicsPutting1996].

## Use when you have already decided to add depth <!-- role: context -->

- **User Goal:** Apply a 3-D treatment to a chart of 2-D data.
- **Task:** Choose among available 3-D renderings.
- **Data:** 2-D quantitative data shown as a line or bar chart.
- **Chart Setting:** A static graph where both 3-D volume and 3-D surface styles are available.
- **Audience:** Viewers judging the chart's appropriateness or memorability.
- **Success Criterion:** The 3-D chart feels more acceptable than a floating-surface alternative.

## Do not use when depth itself is unnecessary <!-- role: exceptions -->

**Break it when:** The chart does not need a 3-D treatment at all. **Why:** This rule only applies after you have already decided to use depth.

## Costs of using solid 3-D volume forms <!-- role: costs -->

**Sacrifice:** Some flat simplicity.
**Risk:** Any 3-D rendering still adds extra structure to a chart of 2-D data.
**Mitigation:** If depth is not serving a communication or memory goal, return to a 2-D rendering instead of choosing among 3-D styles.

## Common misuse of 3-D styling <!-- role: mistakes -->

**Mistake:** Using a floating surface just to signal that the chart is 3-D. **Why it fails:** That 3-D style was less preferred than a solid volume rendering.

## Check the 3-D style choice <!-- role: check -->

**Failure Sign:** The chart uses a surface that appears suspended in space even though a solid volume version is available.
**Quick Check:** Compare volume and surface renderings of the same data and ask which one better fits the communication goal.
**Stronger Test:** If the chart must stay 3-D, keep the version that viewers judge more appropriate; if the chart mainly supports immediate reading or private inspection, step out of the 3-D choice and use a flat version instead.

## Fix the 3-D treatment <!-- role: fix -->

- Fill the 3-D form so it reads as a solid volume rather than a floating surface.
- Replace top-only or suspended surfaces with full 3-D bars or volume-under-the-line forms.
- If the current surface effect is only decorative, remove the 3-D treatment instead of keeping the weaker 3-D style.
