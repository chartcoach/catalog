---
id: explain-that-visible-paths-are-a-sample-not-the-full-set
title: Explain that visible paths are a sample, not the full set
bibliography: references.bib
description: For point-location judgments in static uncertainty forecasts, use explanatory
  instructions on ensemble path maps to improve fidelity and mitigate deterministic
  readings of individual paths for novice viewers.
labels:
- purpose:refine
- basis:empirical
- chart:map
- data:geospatial
- quality:fidelity
- lever:text-annotation
- operator:uncertainty
- literacy:novice
---

## Add a sample-versus-full-set explanation <!-- role: advice -->

Add accompanying instructions that explain how the ensemble display was generated and that the visible paths are only a small sample of many possible model outputs. For example, show a short tutorial that contrasts many model runs with the smaller set plotted in the static image and state that any one visible path is not very meaningful on its own.

## Why the explanation helps <!-- role: reason -->

Without an explanation, viewers can reasonably treat each line as a deterministic route the storm could take. Telling them that the display shows only a subset of many outputs makes the display read more like sampled uncertainty and less like a checklist of exact options.

**Mechanism:** The explanation weakens deterministic construal of individual paths and redirects interpretation toward the distribution that the paths sample.

**Evidence:** In the instruction experiment, a visualization-explanation video reduced the overlap bias in location judgments relative to no instructions, and more viewers correctly rejected the idea that the map showed all possible paths after receiving the explanation [@padillaPowerfulInfluenceMarks2020].

**Notes:** The paper found that this general explanation helped, but did not eliminate the overlap bias.

## Use when all are true <!-- role: context -->

- **User Goal:** Interpret the uncertainty of a forecast path display and judge risk at a specific location.
- **Task:** Read a static ensemble display without full access to the underlying model outputs.
- **Data:** Geospatial uncertainty shown as sampled paths.
- **Chart Setting:** A forecast map shown as a single image, especially when viewers would otherwise receive little background on how it was made.
- **Audience:** Novice viewers or other non-experts.
- **Success Criterion:** Fewer viewers treat single visible paths as decisive or assume the display shows every possible path.

## Do not use when any are true <!-- role: exceptions -->

**Break it when:** Precise location judgments depend on removing overlap bias by itself. **Why:** A general explanation reduced the bias, but left a substantial residual effect.

## Tradeoffs of adding explanation <!-- role: costs -->

**Sacrifice:** The display now requires an onboarding step outside the marks themselves.\
**Risk:** Viewers may feel more confident after the explanation even though some overlap bias remains.\
**Mitigation:** Keep the explanation focused on the sampled nature of the visible paths and test whether the bias actually falls.

## Common failure modes <!-- role: mistakes -->

**Mistake:** Mentioning uncertainty in general without explicitly saying that the visible paths are only a subset of many possible outputs. **Why it fails:** Viewers can still treat the plotted lines as the full set of meaningful routes.

## How to test it <!-- role: check -->

**Failure Sign:** Viewers say the display shows all possible paths or still treat touching a visible path as uniquely important.\
**Quick Check:** Ask viewers whether the display shows all possible paths and whether equal-distance locations should differ just because one touches a visible line.\
**Stronger Test:** Compare matched on-line and off-line location judgments before and after the explanation.

## What to change <!-- role: fix -->

- Add a short explanation of how multiple model outputs lead to the sampled paths shown.
- State explicitly that the static image displays only a subset of many possible paths.
- Contrast the sampled static image with a fuller animation or tutorial view if you can provide one.
