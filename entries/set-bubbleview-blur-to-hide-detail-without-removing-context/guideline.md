---
id: set-bubbleview-blur-to-hide-detail-without-removing-context
title: Set BubbleView blur to hide detail without removing context
bibliography: references.bib
description: For crowdsourced importance measurement on static images, use moderate
  blur on blurred image views to improve fidelity and mitigate missed regions caused
  by excessive loss of context in remote BubbleView studies.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity
- lever:interaction-access
---

## Blur level <!-- role: advice -->

Set blur high enough that text or fine detail cannot be read outside the bubble, but keep enough surrounding structure visible to navigate the image. For example, use a moderate Gaussian blur around 30-50 pixels on browser-sized images and avoid very high blur such as 70 pixels, which removed too much context in the study.

## Why moderate blur works better than extreme blur <!-- role: reason -->

The blur has two jobs at once: it must force clicking for detail, and it must preserve enough context for navigation. Extreme blur breaks the second job and can change which features viewers even notice.

**Mechanism:** Moderate blur removes legible detail while preserving layout cues. That keeps the task focused without making the image impossible to navigate.

**Evidence:** Across the tested BubbleView settings, the paper repeatedly chose blur strong enough to distort text beyond legibility and found that a very high blur of 70 pixels reduced similarity to attention data by eliminating too much context, while blur around 30-50 pixels worked well across datasets [@kimBubbleViewInterfaceCrowdsourcing2017].

## Use when detail should require a click <!-- role: context -->

- **User Goal:** Make viewers click for local detail while still seeing enough global structure to choose where to click next.
- **Task:** Run a blurred-image BubbleView study on static visuals.
- **Data:** Images with text, labels, or fine detail that should only be readable in the revealed bubble.
- **Chart Setting:** Browser-sized image with a fixed blur level across the whole image.
- **Success Criterion:** Important details are unreadable without clicking, but the overall structure remains navigable.

## Do not use when blur destroys or preserves the wrong features <!-- role: exceptions -->

**Break it when:** Critical small features disappear into the blurred background or remain clearly visible without clicking. **Why:** The blur changes what gets clicked, so the resulting map no longer reflects the intended importance judgment.

## Tradeoffs of increasing blur <!-- role: costs -->

**Sacrifice:** Stronger blur reduces contextual cues.
**Risk:** Small features can vanish, or some features can stay visible enough that participants skip clicking them.
**Mitigation:** Pilot the blurred image itself and inspect which elements become unreadable, hidden, or still obvious.

## Common failure mode with blur setting <!-- role: mistakes -->

**Mistake:** Maximizing blur without checking whether viewers can still navigate the image. **Why it fails:** Participants lose context and important regions are skipped for mechanical reasons rather than true lack of importance.

## How to check whether the blur is calibrated <!-- role: check -->

**Failure Sign:** Viewers can read key text without clicking, or important small elements disappear when blurred.
**Quick Check:** Inspect the blurred image alone before launch and verify both legibility loss and preserved structure.
**Stronger Test:** Review early participant clicks against the blurred image and check whether skipped elements were already visible or fully lost in the blur.

## What to change if it is not working <!-- role: fix -->

- Reduce the blur if important small elements disappear into the background.
- Increase the blur if text remains legible without clicking.
- Pilot the blur on representative images from the same dataset instead of only one example.
- Reinspect the blurred image after every blur change before collecting more data.
