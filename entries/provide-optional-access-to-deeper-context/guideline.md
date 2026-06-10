---
id: provide-optional-access-to-deeper-context
title: Provide optional access to deeper context
bibliography: references.bib
description: For explanatory viewing when some viewers may want to investigate further,
  use optional progressive context layers on a chosen chart and its surrounding annotations
  to improve trust and mitigate confusion from missing context for viewers with mixed
  detail needs.
labels:
- purpose:refine
- basis:rhetorical
- quality:trust
- lever:interaction-access
- communication:context
- knowledge:mixed
---

## Optional context layers <!-- role: advice -->

Add an optional path to deeper context without crowding the main view. For example, let viewers move from a simplified overview to a more detailed chart and then raw data, or expose provenance in a caption, annotation, or interactive layer.

## Why optional context reduces confusion and distrust <!-- role: reason -->

Optional context lets different viewers stop at the level they need. People who want only the main message are not overloaded, while curious viewers can verify provenance or inspect added detail when the overview alone is not enough.

**Mechanism:** Optional deeper layers reduce reliance on guesswork. They give viewers a way to resolve uncertainty, check where the data came from, and inspect more detail only when they want it.

**Evidence:** Too little context left some viewers confused or distrustful, and some wanted access to provenance and other context when needed. Practitioners described click-through designs that move from a simplified overview to a detailed chart and then raw data, while experts warned that interaction helps only when it serves a real purpose and lay participants did not report using interactive tools [@koesten_encountering_2025; @schuster_who_2023; @schuster_being_2024].

**Notes:** The added context can be textual or interactive. The key requirement is that more detail is available when curiosity arises.

## Use when viewers may want to dig deeper <!-- role: context -->

- **User Goal:** Understand the main view quickly, then inspect more detail only if needed.
- **Data:** Additional context exists beyond the overview, such as provenance or underlying raw data.
- **Chart Setting:** The primary view is simplified, and the design can expose a secondary layer through captions, annotations, or interaction.
- **Audience:** Viewers have mixed detail needs, including lay viewers who may need more context before they trust the display.
- **Success Criterion:** Curious viewers can reach deeper context when they want it, while others can stay with the overview.

## Do not rely on decorative interaction <!-- role: exceptions -->

- **Break it when:** the added interaction does not reveal meaningful added context. **Why:** interaction for its own sake does not solve the interpretation problem.
- **Break it when:** essential context is available only through an interactive tool that lay viewers must discover on their own. **Why:** lay viewers may not use the tool, so the context remains effectively hidden.

## Costs of optional context layers <!-- role: costs -->

**Sacrifice:** Some context moves out of the primary view, so not every viewer will see it.
**Risk:** If essential explanation or provenance is hidden only in deeper layers, viewers who do not interact can remain confused or distrustful.
**Mitigation:** Keep the overview visible, but make the path to provenance, a more detailed chart, or raw data clear and purposeful.

## Common failure modes for optional context layers <!-- role: mistakes -->

- **Mistake:** Leaving viewers with only a simplified view and no way to inspect provenance or added detail. **Why it fails:** missing context can leave viewers confused or distrustful.
- **Mistake:** Adding interactive controls that do not reveal a clear next level of detail. **Why it fails:** the interaction becomes decorative, and lay viewers may not use it.

## Check whether deeper context is truly reachable <!-- role: check -->

**Failure Sign:** Viewers ask where the data came from or cannot find more detail after reading the overview.
**Quick Check:** Starting from the main view, try to reach provenance or a deeper detail layer in one clear step through a caption, annotation, or interactive layer.
**Stronger Test:** Ask a lay viewer who becomes curious to find the next level of detail; if they do not notice or use the path, the optional context is not truly accessible.

## Fix missing or hidden deeper context <!-- role: fix -->

- Add a clearly labeled path from the simplified overview to a more detailed chart.
- Add optional provenance or explanatory context in a caption, annotation, or secondary layer.
- Add a deeper final layer with raw data for viewers who want to inspect it.
- Remove interactive elements that do not reveal meaningful added context.
