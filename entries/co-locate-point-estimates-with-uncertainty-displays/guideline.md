---
id: co-locate-point-estimates-with-uncertainty-displays
title: Co-locate the point estimate with the uncertainty display
bibliography: references.bib
description: For fast decisions in compact timeline views that show both a point prediction
  and predictive uncertainty, use a spatially co-located point estimate on the uncertainty
  display to improve fidelity and mitigate false precision for novice mobile users.
labels:
- purpose:refine
- basis:empirical
- chart:timeline
- operator:uncertainty
- reading-mode:overview
- quality:fidelity:use
- lever:layout-structure
- literacy:novice
---

## Point estimate placement <!-- role: advice -->

Place the point estimate directly on the uncertainty display so reading the likely value also exposes its uncertainty. For example, move a predicted time off a separate edge-aligned summary position and onto the probability distribution in the same row so viewers do not skim the single number and ignore the spread.

## Why co-locating the point estimate works <!-- role: reason -->

A separated point estimate is easy to skim, but it also makes it easy to ignore uncertainty and act on a false sense of precision. Co-location ties the quick read to the uncertainty view, so the same glance can support both speed and risk awareness.

**Mechanism:** When the point estimate and uncertainty share the same spatial region, attention to the likely value also draws attention to earlier and later possible outcomes. This reduces the chance that viewers treat the prediction as a precise single number.

**Evidence:** During iterative design and informal user testing, a separate right-edge point estimate improved glanceability but let users pay too little attention to the probabilistic estimate; moving the point estimate onto the probability distribution resolved this glanceability versus false-precision tension [@kayWhenIshMy2016].

## When to co-locate the point estimate <!-- role: context -->

- **User Goal:** Make an immediate leave, wait, or detour decision from a forecast.
- **Task:** Read a likely time while also accounting for the chance of earlier or later outcomes.
- **Data:** A point estimate and a predictive distribution for the same future event.
- **Chart Setting:** Compact mobile timeline rows where the display must be glanceable.
- **Audience:** Everyday users making time-constrained decisions with little training.
- **Success Criterion:** Users can read the likely value quickly without ignoring uncertainty.

## When not to co-locate the point estimate <!-- role: exceptions -->

**Break it when:** The view does not need to show a probabilistic estimate alongside the point estimate. **Why:** The benefit of co-location comes from coupling those two readouts in the same glance.

## Tradeoffs of co-locating the point estimate <!-- role: costs -->

**Sacrifice:** You give up some visual separation of the single-number readout.
**Risk:** If the point estimate becomes too subdued on top of the uncertainty display, the view can become harder to skim.
**Mitigation:** Keep the point estimate visible, but keep it inside the same spatial context as the uncertainty display.

## Common mistakes with co-locating the point estimate <!-- role: mistakes -->

**Mistake:** Leaving the point estimate as a separate edge-aligned summary outside the uncertainty display. **Why it fails:** Users can answer from the single number alone and underweight the uncertainty.

## How to check co-locating the point estimate <!-- role: check -->

**Failure Sign:** Users mention only the single predicted time and not the possibility of earlier or later outcomes.
**Quick Check:** Run a short think-aloud with target users; if they can make the decision by reading the isolated number without referring to the uncertainty display, the point estimate is too separable.
**Stronger Test:** Compare a separated version and a co-located version, then keep the one where users mention both the likely value and the surrounding risk.

## How to fix co-locating the point estimate <!-- role: fix -->

- Move the point estimate onto the same mark or region that shows the predictive distribution.
- Remove or demote a separate edge-aligned time summary if it lets users ignore the uncertainty display.
- Align the point estimate within each row so the likely value and the uncertainty are read together.
