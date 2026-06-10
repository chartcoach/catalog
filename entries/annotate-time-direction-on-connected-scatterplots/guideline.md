---
id: annotate-time-direction-on-connected-scatterplots
title: Annotate the direction of time on connected scatterplots
bibliography: references.bib
description: For trend communication in ordered-time paired series, use explicit time-direction
  annotation on connected scatterplots to prevent ambiguous sequence reading and mitigate
  backward interpretations for novice readers.
labels:
- purpose:refine
- basis:empirical
- time:ordered-time
- chart:scatter
- quality:fidelity
- lever:text-annotation
- component:annotation:use
- literacy:novice
---

## Add time-direction cues <!-- role: advice -->

Mark the direction of time directly on the connected path. For example, add arrows, start and end symbols, or point labels so readers do not have to infer the sequence from surrounding text alone.

## Why explicit direction cues work <!-- role: reason -->

Connected scatterplots do not place time on an axis, so the line itself must carry sequence. Without a direction cue, the same shape can support opposite stories.

**Mechanism:** Direct time-direction marks tell readers which point comes first and which way to follow the line, reducing ambiguity when the path loops, crosses itself, or changes direction sharply.

**Evidence:** The paper shows that a connected scatterplot can be drastically misinterpreted without a direction indicator, and the translation study found time reversals in connected-scatterplot reading and copying tasks; it recommends explicit annotation of temporal direction in addition to other cues [@harozConnectedScatterplotPresenting2016].

## Use when the chart must stand alone <!-- role: context -->

- **User Goal:** Communicate how the paired series evolves over time.
- **Task:** Let readers recover the start-to-end sequence from the chart itself.
- **Data:** Two paired time series connected in temporal order.
- **Chart Setting:** A static, self-contained connected scatterplot.
- **Audience:** Readers with little prior experience reading connected scatterplots.
- **Success Criterion:** Readers identify direction correctly without relying on caption text.

## Do not use when motion already provides direction <!-- role: exceptions -->

**Break it when:** Interaction or animation already guides viewers through the sequence. **Why:** The paper notes that motion on the web can help guide readers toward a non-conventional reading direction.

## Costs of adding direction marks <!-- role: costs -->

**Sacrifice:** The chart becomes less visually spare.\
**Risk:** Arrows alone may still not eliminate time reversals.\
**Mitigation:** Combine the annotation with a left-to-right global time flow when possible.

## Common direction-annotation failures <!-- role: mistakes -->

- **Mistake:** Leave direction implicit or explain it only in surrounding text. **Why it fails:** The chart becomes less self-contained and readers can miss critical information.
- **Mistake:** Assume arrows alone fully solve direction confusion. **Why it fails:** Time reversals were still the dominant error pattern in connected-scatterplot tasks.

## Check whether time direction is self-evident <!-- role: check -->

**Failure Sign:** Different readers give opposite start-to-end interpretations of the same line.\
**Quick Check:** Hide the surrounding text and ask a reader to point to the start and end of the path.\
**Stronger Test:** Ask a reader to redraw or verbally replay the sequence from the chart alone and inspect whether the order is reversed.

## Fix ambiguous sequence reading <!-- role: fix -->

- Add arrows along the path to indicate forward time.
- Mark the first and last point with distinct start and end symbols.
- Label points or segments with time labels when the sequence still feels ambiguous.
- If readers still reverse time, reorder the axes so the path flows more clearly from left to right.
