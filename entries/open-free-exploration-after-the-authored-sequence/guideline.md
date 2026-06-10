---
id: open-free-exploration-after-the-authored-sequence
title: Open free exploration after the authored sequence
bibliography: references.bib
description: For interactive data stories, prefer delayed free interaction on narrative
  views to improve insight and mitigate unordered digressions for readers who need
  the main message before exploring.
labels:
- purpose:refine
- basis:empirical
- lever:interaction-access
- quality:insight:use
- communication:workflow
- audience:general-public
---

## Interaction sequencing <!-- role: advice -->

Lead with an authored sequence, then expose broader interaction after the key observations are established. For example, reveal hover details or a time slider after a narrated segment, and place constrained interaction checkpoints inside slides instead of offering unrestricted exploration from the first frame.

## Why delayed exploration works <!-- role: reason -->

Narrative control and exploratory freedom compete for reader attention. Delaying free interaction helps the main message land first, then uses interaction as a continuation of the story rather than as an early distraction.

**Mechanism:** A guided opening establishes the framing questions and the intended reading path before readers branch into their own exploration.

**Evidence:** The analyzed narratives repeatedly used author-driven openings followed by constrained or later-stage interaction, and the paper argues that data stories are most effective when interaction is constrained at checkpoints so readers can explore without veering too far from the intended narrative [@segelNarrativeVisualizationTelling2010].

## Use when the story needs both explanation and exploration <!-- role: context -->

- **User Goal:** Learn the main message, then inspect the data further.
- **Task:** Combine authored storytelling with reader interaction.
- **Chart Setting:** Interactive narratives with hover details, filters, or sliders that could open early or late.
- **Audience:** Readers who need guidance before they can explore productively.
- **Success Criterion:** The main takeaway appears before broad interaction pulls readers into side paths.

## Do not force this sequence at either extreme of the spectrum <!-- role: exceptions -->

**Break it when:** The presentation is purely author-driven with no exploration goal, or purely reader-driven with no authored narrative. **Why:** One case does not need free exploration, and the other does not need a guided opening.

## Costs of delayed exploration <!-- role: costs -->

**Sacrifice:** Readers give up some immediate freedom at the start.\
**Risk:** An overly long authored opening can feel restrictive and delay useful exploration.\
**Mitigation:** Keep the opening only long enough to establish the key questions or themes, then open the view.

## Common failure with delayed exploration <!-- role: mistakes -->

**Mistake:** Exposing unrestricted interaction from the first frame of a dense story. **Why it fails:** Readers can digress into side paths before the intended narrative and key observations are established.

## How to check interaction sequencing <!-- role: check -->

**Failure Sign:** Broad controls are available before the first major point has been communicated.\
**Quick Check:** Inspect the first frame and note whether unrestricted controls appear before the first annotated takeaway.\
**Stronger Test:** Compare the current sequence with a version that opens interaction after the first narrative segment and see which one preserves the main message more reliably.

## How to fix premature exploration <!-- role: fix -->

- Hold advanced controls until after the first annotated or narrated segment.
- Use constrained single-frame interactions inside slides before opening broader exploration.
- Treat narrative checkpoints as the places where new interaction becomes available.
