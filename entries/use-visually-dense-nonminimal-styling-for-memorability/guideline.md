---
id: use-visually-dense-nonminimal-styling-for-memorability
title: Use visually dense, non-minimal styling when memorability is the goal
bibliography: references.bib
description: For short-exposure recall of single static visualizations, use visually
  dense, low-data-ink styling on the chart to improve memorability and mitigate overly
  plain, forgettable displays for viewers scanning many graphics.
labels:
- purpose:refine
- basis:empirical
- quality:insight:use
- lever:encoding
- density:dense
- aesthetic:style:use
---

## Increase density instead of maximizing minimalism <!-- role: advice -->

Use a denser, less minimalist chart image when you want the visualization itself to be remembered. For example, keep more visible detail and allow a lower data-ink ratio instead of stripping the graphic down to a sparse, clean version; in this study, high-density and low-data-ink designs were more memorable than sparse, high-data-ink ones.

## Extra detail creates more distinctive memory cues <!-- role: reason -->

A denser chart gives the viewer more visual features to latch onto, which can make the image stand out from a field of similar sparse charts.

**Mechanism:** Extra visible detail increases distinctiveness during quick viewing, which can improve later recognition of the visualization as an image.

**Evidence:** High visual density scored higher than medium or low density, and low-data-ink-ratio displays scored higher than more minimalist high-data-ink-ratio displays in the memorability experiment [@borkinWhatMakesVisualization2013].

**Notes:** The paper explicitly separates memorability of the chart image from comprehension of the encoded information.

## Use when image recall matters more than minimalism <!-- role: context -->

- **User Goal:** Make a single visualization memorable after a brief glance.
- **Task:** Later recognize the same chart image among many other graphics.
- **Data:** Any data shown in a single-panel static visualization.
- **Chart Setting:** A single-panel static display viewed quickly and without interaction.
- **Audience:** Viewers scanning many charts where sparse designs can look similar.
- **Success Criterion:** Higher repeat recognition and fewer misses.

## Do not use when comprehension is the main requirement <!-- role: exceptions -->

**Break it when:** the display is interactive or multi-panel, or when success depends on understanding the underlying data rather than recognizing the chart image. **Why:** the study measured memorability of single static visualizations as images, and the paper explicitly warns that visual clutter does not necessarily aid comprehension and may interfere with it.

## Denser styling improves recall but adds clutter <!-- role: costs -->

**Sacrifice:** You give up minimalist presentation and a high data-ink ratio.
**Risk:** Added clutter may become what viewers remember instead of the relevant data or trend.
**Mitigation:** Use the added detail only when memorability is the success criterion and keep the most important content visually central.

## Minimalism is not the memory-maximizing default <!-- role: mistakes -->

**Mistake:** Stripping the chart down to maximize data-ink ratio when later recognition is the goal. **Why it fails:** sparse, clean displays were less memorable than denser, lower-data-ink displays.

## Compare sparse and dense versions directly <!-- role: check -->

**Failure Sign:** The chart blends into other graphics after a brief glance.
**Quick Check:** Show a minimalist version and a denser version for about one second in a stream of other charts, then compare repeat-detection hits and false alarms.
**Stronger Test:** Compute d-prime for both versions and keep the denser version only if it improves recognition rather than just raising false alarms.

## Add back detail selectively <!-- role: fix -->

- Add back visible detail or ornament to a stripped-down version.
- Increase the number of visible elements so the display is not unusually sparse.
- Relax high-data-ink simplification when the current chart is forgettable under quick viewing.
