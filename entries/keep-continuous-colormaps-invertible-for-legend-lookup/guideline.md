---
id: keep-continuous-colormaps-invertible-for-legend-lookup
title: Keep continuous colormaps invertible for legend lookup
bibliography: references.bib
description: For legend-based lookup across ordered values, avoid repeated or flat
  color regions on continuous color scales to prevent ambiguous value inversion and
  address non-unique color-to-value mappings for viewers matching colors back to the
  legend.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity:use
- lever:encoding
- polish:palette
- operator:lookup
---

## Global color uniqueness <!-- role: advice -->

Ensure that every position on a continuous color scale maps to a distinct perceptual color when viewers must look values up from the legend. For example, remove flat constant-color spans and duplicated colors across distant parts of the scale so two different values do not read as the same legend entry.

## Why invertibility matters <!-- role: reason -->

If multiple values share the same visible color, a reader cannot reliably map a seen color back to one unique value. The scale then stops working as a lookup device across its full range.

**Mechanism:** Positive minimum local and global speed preserves legend-based order by keeping neighboring and distant values perceptually distinguishable enough to invert color back to value.

**Evidence:** The collated review records this paper as color-encoding theory, and the paper defines legend-based order as invertibility, measured by positive minimum local and global speed; flat or repeated regions break that condition [@zengReviewCollationGraphical2023; @bujackGoodBadUgly2018].

## Use when the legend must decode any color <!-- role: context -->

- **User Goal:** Match a seen color back to a specific ordered value.
- **Task:** Legend-based lookup across the whole scale, not only adjacent comparison.
- **Data:** Ordered values shown with a continuous color scale.
- **Chart Setting:** Static legend where any sampled color may need to be decoded back to value.
- **Audience:** Viewers who use the legend as a readout device rather than only as a rough orientation aid.
- **Success Criterion:** Any visible color maps back to one unique position on the legend.

## Do not use when only local comparison matters <!-- role: exceptions -->

**Break it when:** Readers only compare neighboring values locally and do not need unique lookup from arbitrary colors across the whole scale. **Why:** The paper distinguishes local and global legend-based order, and global invertibility is the stricter requirement.

## Tradeoffs of global uniqueness <!-- role: costs -->

**Sacrifice:** You give up deliberate flat or repeated regions in the palette.
**Risk:** Forcing uniqueness everywhere can conflict with designs that intentionally hold one region constant.
**Mitigation:** Reserve constant-color regions for cases where global legend lookup is not required.

## Common failure with repeated colors <!-- role: mistakes -->

**Mistake:** Reusing the same color at multiple positions or inserting a flat constant-color span while still presenting the scale as continuous. **Why it fails:** A reader cannot invert the seen color back to a single value.

## Check invertibility directly <!-- role: check -->

**Failure Sign:** Two distant values on the scale appear identical or a span shows no visible change.
**Quick Check:** Scan the palette for repeated patches or flat regions with no perceptual movement.
**Stronger Test:** Compute the minimum global speed and require it to stay positive across the sampled scale.

## Fix non-unique color mapping <!-- role: fix -->

- Replace constant-color spans with a continuous perceptual progression.
- Remove duplicated colors that appear at multiple distant positions on the scale.
- Re-sample the palette and verify that every segment shows positive perceptual change.
