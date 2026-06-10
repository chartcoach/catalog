---
id: remove-the-centerline-when-it-overstates-central-impact
title: Remove the centerline when a bounded uncertainty region should not imply peak
  impact at the middle
bibliography: references.bib
description: For intuitive impact judgments across ordered future time, avoid a salient
  centerline on bounded geospatial forecast maps to prevent central-path overemphasis
  and mitigate intensity misreadings for viewers with low domain knowledge.
labels:
- purpose:refine
- basis:empirical
- time:ordered-time
- data:geospatial
- quality:fidelity
- lever:encoding
- operator:uncertainty
- needs:low-domain-knowledge
---

## Centerline removal <!-- role: advice -->

Do not add a prominent centerline inside a bounded uncertainty region when viewers should judge distributed impact rather than a single peak path. For example, use a cone-only or fuzzy-cone uncertainty region instead of a cone-plus-centerline when the line itself is not supposed to signal maximum damage at the middle.

## Why removing the centerline changes judgments <!-- role: reason -->

A centerline acts like a strong axis of impact inside the uncertainty region. Non-expert viewers can overweight that line and treat the middle of the display as more intense, even though the display is meant to communicate track uncertainty rather than peak damage at the center.

**Mechanism:** Removing the line weakens the visual pull toward the middle of the region. This reduces the tendency to equate nearness to the centerline with greater impact.

**Evidence:** At the 24-hour timepoint, cone-only and fuzzy-cone displays both produced lower damage judgments at the center than the cone-centerline display, indicating that the centerline increased perceived central intensity [@ruginskiNonexpertInterpretationsHurricane2016].

**Notes:** The study also found that removing or softening the centerline reduced how strongly some viewers interpreted the display as showing where the eye was likely to travel.

## Use when the middle of the region should not dominate impact judgments <!-- role: context -->

- **User Goal:** Estimate likely impact at locations around a forecast path.
- **Task:** Make intuitive spatial judgments for positions near the center and boundaries of an uncertainty region.
- **Data:** Geospatial path forecasts with positional uncertainty across future times.
- **Chart Setting:** A bounded uncertainty region is already being used on a map.
- **Audience:** Non-expert viewers with low domain knowledge.
- **Success Criterion:** Viewers do not assign disproportionately high impact to the region's middle just because a line is present.

## Do not use when the path-of-eye cue is the priority <!-- role: exceptions -->

**Break it when:** The main goal is to show where the eye or central path is likely to travel. **Why:** Removing or softening the centerline reduced the likelihood that viewers interpreted the display as showing where the eye would go.

## Costs of removing the centerline <!-- role: costs -->

**Sacrifice:** You lose a clear single-path cue.
**Risk:** Viewers may be less likely to read the display as showing the eye's likely path.
**Mitigation:** Use this change when distributed impact judgment matters more than preserving a strong eye-path cue.

## Common failure around this move <!-- role: mistakes -->

**Mistake:** Keep the centerline equally salient while expecting the bounded region to be read as a neutral uncertainty band. **Why it fails:** The centerline can raise perceived impact at the middle of the region.

## Check whether the centerline is overdriving the reading <!-- role: check -->

**Failure Sign:** The center location gets much higher impact judgments than nearby in-region locations.
**Quick Check:** Compare the same bounded region with and without the centerline; if center ratings drop when the line is removed, the line is overdriving interpretation.
**Stronger Test:** Ask viewers whether the display is mainly showing where the eye will travel; if that answer is essential, removing the line may be too aggressive.

## Fix the centerline cue <!-- role: fix -->

- Delete the centerline from the bounded uncertainty region.
- If a bounded region must remain, switch from cone-plus-centerline to cone-only or fuzzy-cone.
- If uncertainty still needs a strong explicit cue after removing the line, replace the bounded region with a multiple-track ensemble instead of restoring the centerline.
