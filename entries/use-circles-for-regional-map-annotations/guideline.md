---
id: use-circles-for-regional-map-annotations
title: Use circles when annotations describe regions rather than points
bibliography: references.bib
description: For explaining regional patterns on a detailed map, use circle annotations
  on the map to improve readability and mitigate overly point-specific arrow callouts
  for readers scanning clusters rather than single marks.
labels:
- purpose:refine
- basis:heuristic
- chart:map
- quality:readability
- lever:text-annotation
- component:annotation:use
- polish:annotation
---

## Use circle annotations for regions <!-- role: advice -->

Use circles when an annotation refers to an area or cluster instead of a single mark. For example, replace arrow pointers with circles when the note describes a regional pattern spread across many mapped points.

## Why circles fit regional claims <!-- role: reason -->

A regional note needs a regional cue. A circle marks an area of related marks without falsely implying that one exact point is the whole story.

**Mechanism:** Circle annotations match the scale of a regional statement, so readers interpret the note as applying to an area instead of a single pinpointed location.

**Evidence:** The post replaces arrows with circles specifically because the annotations describe regional patterns rather than labeling specific data points [@mintzer_map_annotations_2024].

## Use when the annotation refers to an area <!-- role: context -->

- **User Goal:** Explain broad geographic patterns on a map.
- **Task:** Connect annotation text to a region rather than to one exact mark.
- **Data:** Many mapped points forming visible clusters or regional concentrations.
- **Chart Setting:** A detailed map with several explanatory annotations.
- **Audience:** Readers scanning for broad spatial patterns.
- **Success Criterion:** Readers understand that the note applies to a region, not to one isolated point.

## Do not use when the note targets one exact mark <!-- role: exceptions -->

**Break it when:** The annotation is labeling a specific data point. **Why:** A circle is less precise than a point-specific pointer.

## What you trade away <!-- role: costs -->

**Sacrifice:** You give up exact point targeting.\
**Risk:** A circle can feel vague if the note is really about one location.\
**Mitigation:** Reserve circles for regional notes and keep point-specific pointers for point-specific notes.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Use an arrow for annotation text that describes a broad regional pattern. **Why it fails:** The arrow suggests one exact target even though the claim applies to many marks.

## How to test it <!-- role: check -->

**Failure Sign:** The annotation text uses regional language, but the connector ends at one point.\
**Quick Check:** Ask whether the note describes a cluster or a single mark.\
**Stronger Test:** Compare an arrow version and a circle version and keep the one whose connector matches the geographic scope of the statement.

## What to change <!-- role: fix -->

- Replace arrow connectors with circles around the relevant region.
- Keep arrows only for annotations that label a single specific point.
- Rewrite or position the annotation so its text clearly refers to the circled area.
