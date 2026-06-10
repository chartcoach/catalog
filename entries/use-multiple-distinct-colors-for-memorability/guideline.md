---
id: use-multiple-distinct-colors-for-memorability
title: Use multiple distinct colors when memorability is the goal
bibliography: references.bib
description: For short-exposure recall of single static visualizations, use multiple
  distinct colors on the chart to improve memorability and mitigate bland, easily
  confusable displays for viewers scanning many graphics.
labels:
- purpose:refine
- basis:empirical
- quality:insight:use
- lever:encoding
- aesthetic:color:use
- channel:color-hue:use
---

## Increase distinct color variety <!-- role: advice -->

Use more distinct colors when you want the visualization itself to be remembered. For example, move from a one-color or black-and-white scheme to a palette with several distinct hues; displays with seven or more distinct colors were more memorable than displays with one color or only a few colors.

## Distinct colors make charts easier to discriminate <!-- role: reason -->

Distinct colors give a chart image more separable visual cues, so it is easier to recognize again instead of confusing it with similar graphics.

**Mechanism:** More color increases visual distinctiveness during quick viewing, which helps later recognition of the chart image.

**Evidence:** Visualizations with seven or more colors had higher memorability scores than those with two to six colors, and both outperformed one-color displays; this color effect remained statistically significant even after removing visualizations containing pictograms [@borkinWhatMakesVisualization2013].

## Use when the chart must stand out in a stream <!-- role: context -->

- **User Goal:** Make a single visualization easier to remember after a short exposure.
- **Task:** Later recognize the same chart image among many other graphics.
- **Data:** Any data shown in a single-panel static visualization.
- **Chart Setting:** A single-panel static display viewed quickly and without interaction.
- **Audience:** Viewers scanning many graphics in sequence.
- **Success Criterion:** Higher repeat recognition and lower confusion with similar charts.

## Do not use when the study conditions do not match <!-- role: exceptions -->

**Break it when:** the display is interactive or multi-panel, or when success depends on understanding the underlying data rather than recognizing the chart image. **Why:** the study measured memorability of single static visualizations as images and did not show that extra color improves comprehension.

## More color improves recall but weakens restraint <!-- role: costs -->

**Sacrifice:** You give up a restrained monochrome look.
**Risk:** Viewers may remember the palette as an image cue more than the data meaning carried by the colors.
**Mitigation:** Use the added colors when memorability is the goal, not as a default assumption that the chart is easier to understand.

## Monochrome charts are easy to overlook in memory <!-- role: mistakes -->

**Mistake:** Keeping the chart monochrome and expecting it to stand out in memory. **Why it fails:** one-color displays were the least memorable color group in the study.

## Compare the palette with a quick memory test <!-- role: check -->

**Failure Sign:** Viewers confuse the chart with other graphics after a brief glance.
**Quick Check:** Show a monochrome version and a multicolor version for about one second in a stream of other charts, then compare repeat-detection hits and false alarms.
**Stronger Test:** Compute d-prime for both versions and keep the palette that raises recognition without increasing confusion.

## Revise the palette toward distinct hues <!-- role: fix -->

- Replace a one-color or black-and-white scheme with several distinct hues.
- If the current palette uses only a few colors, test a version with more distinct colors.
- Keep the added colors visually distinct so the chart is less confusable at a glance.
