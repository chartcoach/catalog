---
id: use-color-hue-instead-of-shape-for-nominal-categories
title: Use color hue instead of shape to encode nominal categories
bibliography: references.bib
description: For category differentiation in color-capable static charts with categorical
  data, prefer color hue encoding on marks to improve fidelity and mitigate weak group
  separation for readers identifying categories.
labels:
- purpose:refine
- basis:empirical
- data:categorical
- quality:fidelity
- lever:encoding
- channel:color-hue:use
- channel:shape:avoid
---

## Hue encoding for category identity <!-- role: advice -->

Encode the nominal field with color hue instead of shape when distinct colors are available. For example, distinguish groups by different hues rather than by changing point or mark shapes for the same categorical field.

## Why hue works better than shape here <!-- role: reason -->

Nominal data needs readers to tell categories apart without implying order. Distinct hues provide a stronger nominal encoding than shape for that job.

**Mechanism:** Color hue separates categories more effectively than shape for the same nominal field.

**Evidence:** The collated knowledge records Mackinlay's nominal effectiveness ranking as positionX = positionY > color-hue > texture > color-saturation > shape > length > angle > orientation > area, so color hue is the stronger encoding choice over shape for nominal data [@zengReviewCollationGraphical2023; @mackinlayAutomatingDesignGraphical1986].

## Use when the output can show color <!-- role: context -->

- **User Goal:** Distinguish categories accurately.
- **Data:** One categorical field with no intrinsic order is being assigned to a visual channel.
- **Chart Setting:** A static 2D chart with marks is being designed, and the output medium can show color.
- **Success Criterion:** Readers can tell categories apart directly from the marks.

## Do not use when color is unavailable <!-- role: exceptions -->

**Break it when:** The output medium is monochrome or cannot reliably show color. **Why:** This guideline depends on color hue being available as the encoding channel.

## Costs of moving the field to hue <!-- role: costs -->

**Sacrifice:** Hue uses the color channel.
**Risk:** If color is unavailable, the rule cannot be applied directly.
**Mitigation:** Use another nominal channel only after color has been ruled out by the medium.

## Common failure around this choice <!-- role: mistakes -->

**Mistake:** Distinguish the main categories only with shapes when distinct hues are available. **Why it fails:** It leaves the nominal field on a lower-ranked channel than hue.

## Check the encoding decision directly <!-- role: check -->

**Failure Sign:** Readers must inspect mark shapes to tell categories apart.
**Quick Check:** Recolor the same categories with distinct hues and see whether the grouping can be read without inspecting shapes.
**Stronger Test:** If the hue version expresses the same grouping, keep hue and simplify the shapes.

## Fix the channel assignment <!-- role: fix -->

- Map the categorical field to distinct hues.
- Return marks to a common shape when shape no longer carries the grouping.
- If color is not available, move the grouping to another nominal channel rather than leaving the design dependent on hue.
