---
id: do-not-rely-on-fuzzy-boundaries-alone-to-fix-cone-misreadings
title: Do not rely on boundary softness alone to correct bounded uncertainty displays
bibliography: references.bib
description: For intuitive impact judgments across ordered future time, avoid using
  boundary softness alone on bounded geospatial forecast maps to prevent false confidence
  in improved comprehension and address persistent size-and-distance misreadings for
  viewers with low domain knowledge.
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

## Boundary softness alone <!-- role: advice -->

Do not assume that blurring the edges of a bounded uncertainty region will, by itself, fix intuitive misreadings. For example, changing a hard-bounded cone to a fuzzy cone still left the main time-and-distance judgment pattern close to the standard cone display.

## Why fuzzy edges are not enough here <!-- role: reason -->

Soft edges change appearance, but they leave the same widening bounded shape in place. If the main misread comes from the growing region and its spatial form, boundary softness alone will not change the underlying interpretation very much.

**Mechanism:** A soft boundary can shift attention to color depth, but it does not remove the widening region or the spatial center that viewers use to infer size and impact.

**Evidence:** The fuzzy-cone display showed no strong change in the distance effect relative to the cone-centerline, and changes in damage judgments from 24 to 48 hours were similar across those displays [@ruginskiNonexpertInterpretationsHurricane2016].

**Notes:** Fuzzy boundaries did produce some local changes, including more attention to color depth and less agreement that the display showed where the eye would travel.

## Use when you are revising a cone-based uncertainty display <!-- role: context -->

- **User Goal:** Improve intuitive understanding of uncertainty in a bounded forecast region.
- **Task:** Reduce misreadings tied to distance from center and increasing forecast time.
- **Data:** Geospatial forecast uncertainty shown as a bounded region that widens over time.
- **Chart Setting:** A cone-like uncertainty region is already being used on a static map.
- **Audience:** Non-expert viewers with low domain knowledge.
- **Success Criterion:** The revision materially changes how viewers judge uncertainty, not just how the boundary looks.

## Do not use as a warning when your goal is narrower <!-- role: exceptions -->

**Break it when:** Your only goal is to reduce how strongly the display is read as a specific eye path or to make viewers attend more to color depth. **Why:** The fuzzy boundary did affect those specific cues even though it did not strongly improve the broader damage-judgment pattern.

## Costs of rejecting the fuzzy-edge-only fix <!-- role: costs -->

**Sacrifice:** You give up an easy minimal restyle.
**Risk:** A more effective correction may require a larger redesign of the uncertainty encoding.
**Mitigation:** Judge the revision by whether it changes time and distance interpretations, not by whether the boundary looks more uncertain.

## Common failure around this move <!-- role: mistakes -->

**Mistake:** Blur the cone edges and stop there. **Why it fails:** The same widening bounded form remains, so viewers can still read later forecasts as larger or more damaging.

## Check whether the softer edge actually changed interpretation <!-- role: check -->

**Failure Sign:** Viewers still show nearly the same impact pattern across time and distance after the boundary is softened.
**Quick Check:** Compare the current hard-bounded cone with a fuzzy version; if later timepoints still read as greater impact and center-distance judgments barely move, the soft edge did not solve the problem.
**Stronger Test:** Ask viewers whether the event seems larger or more damaging at later times; if that response persists, boundary softness was not enough.

## Fix the revision strategy <!-- role: fix -->

- Do not stop at changing edge hardness or blur.
- Replace the bounded cone with a different uncertainty encoding, such as multiple plausible paths.
- Re-check early and later forecast times after the redesign to confirm that the later view no longer inflates perceived impact by itself.
