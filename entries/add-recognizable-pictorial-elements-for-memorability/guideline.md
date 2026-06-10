---
id: add-recognizable-pictorial-elements-for-memorability
title: Add recognizable pictorial elements when memorability is the goal
bibliography: references.bib
description: For short-exposure recall of single static visualizations, use pictorial
  annotation on the chart to improve memorability and mitigate forgettability for
  viewers scanning many graphics.
labels:
- purpose:refine
- basis:empirical
- quality:insight:use
- lever:encoding
- component:annotation:use
- aesthetic:style:use
---

## Add pictorial annotation <!-- role: advice -->

Add a human-recognizable pictorial element when you want the visualization itself to stick in memory. For example, use a cartoon, photograph, logo, or other recognizable object as part of the chart image instead of leaving the display entirely abstract.

## Recognizable objects create strong memory cues <!-- role: reason -->

Recognizable objects are easy to segment and identify quickly, so they give a chart image a distinctive cue that survives brief viewing.

**Mechanism:** A recognizable picture gives the viewer a concrete visual anchor, which makes the chart easier to recognize again and less likely to be confused with other graphics.

**Evidence:** Visualizations containing human-recognizable pictograms had substantially higher memorability scores than those without them, and nearly all of the top overall examples contained recognizable cartoons or images [@borkinWhatMakesVisualization2013].

**Notes:** The paper treated photographs, cartoons, logos, and similar recognizable objects as pictorial elements.

## Use when chart-image recall matters <!-- role: context -->

- **User Goal:** Make a single visualization memorable after a brief glance.
- **Task:** Later recognize the same chart image among many other graphics.
- **Data:** Any data shown in a single-panel static visualization.
- **Chart Setting:** A single-panel static display viewed quickly and without interaction.
- **Audience:** Viewers encountering many visualizations in sequence.
- **Success Criterion:** Higher repeat recognition with fewer confusions.

## Do not use when image recall is not the target <!-- role: exceptions -->

**Break it when:** the display is interactive or multi-panel, or when success depends on understanding the underlying data rather than recognizing the chart image. **Why:** the study measured memorability of single static visualizations as images and did not show that this move improves comprehension.

## Pictorial annotation trades abstraction for recall <!-- role: costs -->

**Sacrifice:** You give up some visual abstraction and minimalism.
**Risk:** Viewers may remember the picture more strongly than the intended data message.
**Mitigation:** Make the pictorial element relevant to the point you want to stick rather than adding unrelated decoration.

## Generic decoration is not the same thing <!-- role: mistakes -->

**Mistake:** Adding generic decorative clutter instead of a recognizable object. **Why it fails:** the observed gain came from human-recognizable images, not from decoration in general.

## Test whether the picture improves recognition <!-- role: check -->

**Failure Sign:** Viewers miss the chart when it reappears or confuse it with similar charts.
**Quick Check:** Show pictorial and non-pictorial versions for about one second in a stream of other graphics, then compare repeat-detection hits and false alarms.
**Stronger Test:** Compute d-prime for both versions and keep the version with the higher score.

## Edit the chart image toward recognizability <!-- role: fix -->

- Add one recognizable object, cartoon, photo, or logo to the chart image.
- Replace generic decorative shapes with a pictorial element viewers can identify quickly.
- If the chart already has embellishment, make at least one embellishing element clearly human-recognizable.
