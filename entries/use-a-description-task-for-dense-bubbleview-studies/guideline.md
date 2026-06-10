---
id: use-a-description-task-for-dense-bubbleview-studies
title: Use a description task for dense BubbleView studies
bibliography: references.bib
description: For small-sample crowdsourced importance measurement, use a description
  task on dense static visuals to improve fidelity and mitigate diffuse click patterns
  in remote BubbleView studies.
labels:
- purpose:refine
- basis:empirical
- density:dense
- quality:fidelity
- lever:interaction-access
---

## Description task <!-- role: advice -->

Add a description task when the visual has enough semantic or textual content to describe and you need reliable importance maps from few participants. For example, ask viewers to click and type a short description for an information visualization or webpage instead of only free-viewing it, and use the submitted text to screen out poor trials.

## Why the description task sharpens clicks <!-- role: reason -->

A description task changes where viewers spend effort. They click more selectively on regions that help them complete the task, so informative regions emerge with fewer participants.

**Mechanism:** Typing while clicking adds an effort barrier. That barrier reduces casual exploration and concentrates clicks on task-relevant areas that support the written description.

**Evidence:** BubbleView performed best on information visualizations with a description task, and on webpages the description task produced better fixation approximation than free viewing for small participant counts while also enabling description-based quality control [@kimBubbleViewInterfaceCrowdsourcing2017].

**Notes:** The paper recommends BubbleView especially for defined tasks rather than unconstrained viewing.

## Use when the visual has a describable message <!-- role: context -->

- **User Goal:** Approximate eye fixations or recover the most important regions of a static visual.
- **Task:** Run a remote BubbleView study with limited participants.
- **Data:** Dense static images with readable text, labels, or a main message that can be summarized.
- **Chart Setting:** Blurred image with click-to-reveal bubbles and a text field for the response.
- **Success Criterion:** Important regions stabilize quickly and poor-quality responses can be filtered.

## Do not use when the image is not meaningfully describable <!-- role: exceptions -->

**Break it when:** The image cannot be objectively described or requires outside context to interpret. **Why:** The task stops matching the visual, so description quality becomes hard to judge and the clicks no longer cleanly reflect importance.

## Tradeoffs of adding a description task <!-- role: costs -->

**Sacrifice:** The task takes much longer and costs more than short free-viewing.
**Risk:** The task can bias clicks toward the regions needed for the written summary, especially text-heavy regions.
**Mitigation:** Reserve the description task for visuals with a clear message and enough content to describe.

## Common failure mode with the task choice <!-- role: mistakes -->

**Mistake:** Using free-viewing on dense visuals when you only have a small participant pool. **Why it fails:** The click maps converge more slowly, so the important regions remain noisier for the same sample size.

## How to check whether the task is working <!-- role: check -->

**Failure Sign:** Early click maps stay diffuse and the written responses are vague or incomplete.
**Quick Check:** Read a small batch of descriptions and confirm that they mention the main content of the image.
**Stronger Test:** Compare hotspot stability from the first 10-12 participants under the description task versus a free-viewing pilot.

## What to change if it is not working <!-- role: fix -->

- Replace a free-viewing instruction with a click-and-describe instruction.
- Require a minimum response length before participants can continue.
- Remove trials with poor descriptions before building the click map.
- Give participants unlimited or longer viewing time so they can alternate between clicking and writing.
