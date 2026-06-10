---
id: annotate-representative-tracks-with-size-and-intensity
title: Annotate representative tracks with size and intensity
bibliography: references.bib
description: For risk judgments from uncertain geospatial paths over ordered time,
  use size and intensity annotations on representative track displays to improve fidelity
  and mitigate overfocus on the center path for viewers with low domain knowledge.
labels:
- purpose:refine
- basis:empirical
- time:ordered-time
- data:geospatial
- measure:multi
- lever:encoding
- knowledge:low
- quality:fidelity
---

## Risk-variable annotations on representative tracks <!-- role: advice -->

Annotate representative tracks with the forecast variables viewers need for risk judgments instead of leaving the paths unannotated. For example, color track segments by intensity and add periodic size circles along selected tracks so a 15-track display carries path, size, and intensity information together.

## Why size and intensity annotations work <!-- role: reason -->

Risk judgments depend on more than path position alone. Adding size and intensity to the track display lets readers combine uncertainty spread with the local severity of the event at each point along the forecast.

**Mechanism:** Annotations reduce over-reliance on the center path and let viewers calibrate judgments using both the spread of possible paths and the forecast hazard attributes attached to those paths.

**Evidence:** In the paper’s experiment, a 15-track annotated display changed the distance-to-damage relationship relative to a 15-track unannotated display, with lower damage judgments near the center and higher judgments far from the center, indicating better use of spatial uncertainty. Within the annotated display, both forecast size and forecast intensity significantly increased damage ratings, and the 15-track annotated display made viewers more cognizant of spatial spread than a 63-track unannotated display [@liuVisualizingUncertainTropical2019].

## When to add size and intensity annotations <!-- role: context -->

- **User Goal:** Judge likely damage or hazard at a location from an uncertain path forecast.
- **Task:** Combine uncertainty, size, and intensity in one overview display.
- **Data:** A geospatial path ensemble with time-sampled ancillary variables such as size and intensity.
- **Chart Setting:** A representative-track display where track count is kept low enough to leave room for visible annotations.
- **Audience:** Viewers with low prior domain knowledge.
- **Success Criterion:** Judgments reflect both wider uncertainty and stronger or larger forecast conditions.

## When annotation alone is not enough <!-- role: exceptions -->

**Break it when:** Recognizing that spatial spread grows over time is the main goal and the display is limited to only 15 annotated tracks. **Why:** The study found that 15 annotated tracks improved awareness of spread, but the early and late forecast slopes stayed roughly parallel, and the authors indicated that more than 15 annotated tracks may be needed to better show widening spread over time.

## Costs of adding annotations <!-- role: costs -->

**Sacrifice:** You give up some visual simplicity.
**Risk:** With too few annotated tracks, readers may still miss how much the uncertainty widens later in the forecast.
**Mitigation:** Increase the number of annotated tracks if time-dependent growth in spread must be read clearly.

## Common annotation mistake <!-- role: mistakes -->

**Mistake:** Keeping representative tracks unannotated when viewers must judge risk from both path uncertainty and hazard attributes. **Why it fails:** Readers cannot use size and intensity differences that materially affect damage estimates.

## How to check annotations <!-- role: check -->

**Failure Sign:** Risk judgments barely change across forecasts with different size or intensity, or the outer tracks still seem irrelevant.
**Quick Check:** Compare annotated and unannotated versions at the same track count; the annotated version should make both hazard changes and outer-path uncertainty more interpretable.
**Stronger Test:** Ask viewers to rate risk for forecasts that differ in size and intensity at the same offset from the center; ratings should rise with both attributes.

## How to fix missing or weak annotations <!-- role: fix -->

- Color each track segment by the predicted intensity category.
- Add size circles at spaced time intervals along selected tracks.
- Keep enough spacing between tracks so the annotations remain legible.
- If readers still underread later-time spread, add more annotated tracks rather than removing the annotations.
