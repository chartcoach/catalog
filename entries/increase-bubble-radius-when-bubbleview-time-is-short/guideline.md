---
id: increase-bubble-radius-when-bubbleview-time-is-short
title: Increase bubble radius when BubbleView viewing time is short
bibliography: references.bib
description: For short-time crowdsourced importance measurement, use a larger bubble
  radius on dense static visuals to improve fidelity and mitigate undersampling caused
  by tiny focal windows in remote BubbleView studies.
labels:
- purpose:refine
- basis:empirical
- time:time-interval
- density:dense
- quality:fidelity
- lever:interaction-access
---

## Bubble radius for short sessions <!-- role: advice -->

Increase bubble radius when each image is shown only briefly. For example, on dense webpage-like images viewed for about 10 seconds, use a roughly 50-70 pixel bubble instead of a 30 pixel bubble so each click reveals enough context to sample the page.

## Why a larger bubble helps under time pressure <!-- role: reason -->

A short timer limits how many clicks a viewer can make. If each click reveals too little, participants spend their time on mechanical exploration instead of reaching the most informative regions.

**Mechanism:** A larger bubble exposes more content per click. That reduces the number of clicks needed to cover dense layouts before the timer ends.

**Evidence:** On webpage images, BubbleView with 10 seconds of viewing performed worse with a 30-pixel bubble than with 50- or 70-pixel bubbles, and the paper reports that larger bubbles compensate when less time is available [@kimBubbleViewInterfaceCrowdsourcing2017].

## Use when the timer is tight <!-- role: context -->

- **User Goal:** Approximate where viewers would look on a dense static visual.
- **Task:** Run a timed free-viewing BubbleView study.
- **Data:** Dense page-like layouts with many potential targets.
- **Chart Setting:** Blurred image with a fixed short viewing interval per image.
- **Success Criterion:** Participants can expose the important regions before time expires.

## Do not use when viewers already have longer time <!-- role: exceptions -->

**Break it when:** The viewing interval is substantially longer, such as the 30-second condition tested in the paper. **Why:** Very large bubbles then expose too much at once and reduce selectivity, which lowered performance relative to smaller bubbles.

## Tradeoffs of increasing bubble radius <!-- role: costs -->

**Sacrifice:** You give up some spatial precision in the resulting importance map.
**Risk:** A bubble that is too large can blur together nearby targets and reduce selectivity.
**Mitigation:** Increase the bubble only enough to match the available time, or extend the time instead.

## Common failure mode with bubble size <!-- role: mistakes -->

**Mistake:** Keeping a very small bubble in a short timed session. **Why it fails:** Participants spend their limited time opening adjacent small regions instead of reaching the important parts of the image.

## How to check whether the bubble is too small <!-- role: check -->

**Failure Sign:** Participant traces show many adjacent clicks and key regions remain unopened when the timer ends.
**Quick Check:** Inspect a few participant sessions and see whether they are still doing local exploration at timeout.
**Stronger Test:** Pilot two bubble sizes and keep the one that yields a more stable hotspot map within the same short interval.

## What to change if it is not working <!-- role: fix -->

- Increase the bubble radius by one step and rerun a pilot.
- Keep the blur constant while adjusting the bubble so you isolate the time-radius tradeoff.
- If the bubble cannot grow without losing precision, lengthen the viewing interval.
- Recheck whether important regions are reached before the timer ends.
