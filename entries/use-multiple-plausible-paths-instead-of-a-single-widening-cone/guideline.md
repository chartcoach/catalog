---
id: use-multiple-plausible-paths-instead-of-a-single-widening-cone
title: Use multiple plausible paths instead of a single widening cone to show track
  uncertainty
bibliography: references.bib
description: For intuitive impact judgments across ordered future time, use a multiple-instance
  uncertainty encoding on geospatial forecast maps to improve fidelity and mitigate
  misreadings of forecast uncertainty as storm growth for viewers with low domain
  knowledge.
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

## Multiple-path uncertainty encoding <!-- role: advice -->

Show uncertainty with many plausible paths rather than one widening bounded region when non-experts must judge likely impact over time. For example, replace a cone-plus-centerline overlay with an ensemble of multiple forecast tracks on the same map, instead of using a single hard-bounded cone that widens at later timepoints.

## Why multiple paths work here <!-- role: reason -->

A widening bounded region invites a size reading. Showing many possible paths keeps attention on spread and variation instead of on one growing shape, so later forecast times are less likely to be mistaken for a larger or more damaging event.

**Mechanism:** Multiple path instances make uncertainty visible as dispersion. This reduces reliance on the cone's widening shape and lowers the chance that viewers treat increased forecast horizon as increased size or intensity.

**Evidence:** Compared with the cone-centerline display, the ensemble display led to lower damage ratings at the later timepoint, a more distributed effect of distance, and fewer endorsements that the hurricane or its damage gets larger over time [@ruginskiNonexpertInterpretationsHurricane2016].

**Notes:** In think-aloud responses, viewers of the ensemble often shifted to heuristics based on counting visible tracks and judging color depth.

## Use when impact judgments depend on uncertainty interpretation <!-- role: context -->

- **User Goal:** Judge likely impact or damage at locations near a forecast path.
- **Task:** Make intuitive judgments under positional and temporal uncertainty across future forecast times.
- **Data:** Geospatial track forecasts with uncertainty that changes over time.
- **Chart Setting:** A static map with one uncertainty overlay and little or no explanatory legend.
- **Audience:** Non-expert viewers with low domain knowledge.
- **Success Criterion:** Viewers do not infer that the event becomes larger or more damaging solely because the forecast horizon is later.

## Do not use when the audience is outside the tested population <!-- role: exceptions -->

**Break it when:** The audience is domain experts or people with direct hurricane experience rather than low-knowledge novice viewers. **Why:** The evidence comes from non-expert student participants making intuitive judgments with minimal display instruction.

## Costs of switching to multiple paths <!-- role: costs -->

**Sacrifice:** You give up a single dominant center-path cue.
**Risk:** Viewers may replace one shortcut with another and use a simple count-the-tracks heuristic.
**Mitigation:** Use this change when uncertainty communication is the primary goal, not when a single central path must dominate the reading.

## Common failure around this move <!-- role: mistakes -->

**Mistake:** Keep a widening cone as the main uncertainty cue and expect viewers to read it only as greater forecast uncertainty over time. **Why it fails:** Viewers can read the wider later region as a larger or more damaging event.

## Check whether the cone is being read as growth <!-- role: check -->

**Failure Sign:** Later forecast times receive higher impact judgments at the same central location simply because the uncertainty region gets wider.
**Quick Check:** Compare the current cone-based map with a multiple-path version using the same geography and forecast times; if only the cone version makes the later time seem larger or more damaging, the current encoding is distorting uncertainty.
**Stronger Test:** Ask viewers whether the display suggests that the event gets larger or that the damage extent grows over time.

## Fix the uncertainty overlay <!-- role: fix -->

- Replace the single cone-plus-centerline overlay with multiple plausible track lines.
- Remove the widening bounded region as the main cue for uncertainty spread.
- Re-test early and later forecast times after the change to confirm that later time no longer inflates impact judgments by itself.
