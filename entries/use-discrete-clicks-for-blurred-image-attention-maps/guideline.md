---
id: use-discrete-clicks-for-blurred-image-attention-maps
title: Use discrete clicks for blurred-image attention maps
bibliography: references.bib
description: For crowdsourced approximation of visual attention on static images,
  use discrete click collection on blurred image views to improve fidelity and mitigate
  transition noise in remote importance-mapping studies.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity
- lever:interaction-access
---

## Click collection <!-- role: advice -->

Collect discrete clicks instead of continuous mouse movements when you want an importance map from a blurred image. For example, use click-to-reveal bubbles rather than recording every mouse path so the data captures deliberate points of interest instead of transitions between them.

## Why clicks are cleaner than movement traces <!-- role: reason -->

Continuous movement records both destinations and the paths between them. Clicks remove most of that transition noise and turn each sample into an explicit choice.

**Mechanism:** Clicking adds a small effort cost. That cost makes viewers more selective, so the collected samples align better with the regions they consciously choose to inspect.

**Evidence:** BubbleView clicks matched or exceeded continuous mouse-movement approaches at approximating eye fixations on natural images for feasible participant counts, and the paper shows that movement data includes noisy transition traces that require post-processing [@kimBubbleViewInterfaceCrowdsourcing2017].

**Notes:** The paper also reports lower computational and post-processing cost for click collection.

## Use when you need selective importance signals <!-- role: context -->

- **User Goal:** Recover the most important regions of a static image or approximate eye fixations remotely.
- **Task:** Run a mouse-contingent blurred-image study online.
- **Chart Setting:** Click-to-reveal or move-to-reveal interface on a static image.
- **Success Criterion:** The map highlights deliberate regions of interest with fewer participants and less post-processing.

## Do not use when broad coverage matters more than selectivity <!-- role: exceptions -->

**Break it when:** You need broader sampling of image regions rather than only the most important ones. **Why:** Clicking is more selective, so some regions that would receive a quick glance or pass of the mouse may never be sampled.

## Tradeoffs of collecting clicks <!-- role: costs -->

**Sacrifice:** Clicking is slower than moving the mouse.
**Risk:** Fewer regions may be explored in the same amount of time.
**Mitigation:** Give participants more time per image when broad coverage still matters.

## Common failure mode with movement data <!-- role: mistakes -->

**Mistake:** Treating all continuous mouse samples as equally meaningful points of interest. **Why it fails:** The raw path contains transitions between destinations, not just the destinations themselves.

## How to check whether movements are adding noise <!-- role: check -->

**Failure Sign:** Raw traces form long arcs and loops between a small number of hotspots.
**Quick Check:** Visually inspect a few raw sessions and look for path-like traces between meaningful regions.
**Stronger Test:** Compare how many participants are needed before the hotspot map stabilizes under clicks versus movements.

## What to change if it is not working <!-- role: fix -->

- Replace continuous reveal with click-to-reveal bubbles.
- If you must keep movement data, convert the trajectories into discrete points of interest before analysis.
- Increase the viewing time to offset the slower pace of clicking.
- Rebuild the map from the discrete selections rather than from the full paths.
