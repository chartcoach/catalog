---
id: use-lightness-shades-when-totals-matter
title: Use lightness shades of one hue when totals matter more than parts
bibliography: references.bib
description: For part-whole charts with many categories, use color-lightness variation
  within one hue on category parts to improve readability and address overly confetti-like
  palettes for readers who should notice totals before parts.
labels:
- purpose:refine
- basis:heuristic
- lever:encoding
- channel:color-lightness:use
- operator:part-whole
- group-cardinality:many
- quality:readability:use
- polish:palette
---

## Simplify the palette with lightness <!-- role: advice -->

Replace many hues with darker and lighter shades of one hue when you want totals to dominate. For example, use shaded segments in a stacked bar chart instead of a many-hue palette so the total bars read first and the parts stay visible.

## Shift attention from parts to totals <!-- role: reason -->

A one-hue lightness scale reduces color variety while preserving separation between categories. It also changes emphasis: readers notice the overall total more readily, while the individual parts recede compared with a multi-hue palette.

**Mechanism:** Lightness variation keeps categories distinguishable enough to read, but it weakens part-to-part contrast and makes the full bar or total more visually prominent.

**Evidence:** The post recommends darker and lighter versions of one hue to make charts less confetti-like, and it explicitly notes that this shifts focus toward totals and away from parts, especially in stacked bar charts [@muth_fewer_colors_2022].

## Use when totals should read first <!-- role: context -->

- **User Goal:** Reduce palette complexity while keeping parts visible.
- **Task:** Show totals and their parts, with totals carrying more weight.
- **Data:** Many categorical parts are shown inside larger totals.
- **Chart Setting:** A part-whole chart such as a stacked bar chart.
- **Audience:** Readers who should grasp the overall total quickly.
- **Success Criterion:** Totals stand out without making all parts identical.

## Do not use when parts are as important as totals <!-- role: exceptions -->

**Break it when:** Readers need the parts to be as important as or more important than the totals. **Why:** Shades are harder to tell apart than different hues and will push attention away from the parts.

## Accept weaker part separation <!-- role: costs -->

**Sacrifice:** You give up some part-to-part distinctness.
**Risk:** Readers may struggle to compare individual categories closely.
**Mitigation:** Keep different hues when the parts themselves are the main story.

## Avoid using shades for part-heavy reading <!-- role: mistakes -->

**Mistake:** Switching to same-hue shades when the main job is to compare the parts against each other. **Why it fails:** The palette reduces the contrast that those comparisons need.

## Compare focus before and after the palette change <!-- role: check -->

**Failure Sign:** The chart still feels confetti-like even though totals should be the main read.
**Quick Check:** Compare a many-hue version with a one-hue shaded version and see whether totals become more prominent.
**Stronger Test:** Ask whether the palette change has made the parts harder to tell apart than the task allows.

## Edit the palette toward one hue <!-- role: fix -->

- Replace multiple category hues with darker and lighter versions of a single hue.
- Review whether the totals now read first.
- Return to different hues if the parts need stronger visual separation.
