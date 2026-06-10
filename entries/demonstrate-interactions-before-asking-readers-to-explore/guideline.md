---
id: demonstrate-interactions-before-asking-readers-to-explore
title: Demonstrate interactions before asking readers to explore
bibliography: references.bib
description: For interactive narrative views, use interaction cues and tacit tutorials
  on controls to improve readability and address hidden functionality for novice readers.
labels:
- purpose:refine
- basis:empirical
- lever:interaction-access
- quality:readability:use
- literacy:novice
- audience:general-public
- communication:workflow
---

## Interaction cues and tacit tutorials <!-- role: advice -->

Teach the first interaction through the interface before asking readers to explore on their own. For example, animate a slider along with the story so readers learn how to scrub it, place a short prompt or pointer next to an interactive list or start button, and mark interactive components so they are visibly clickable.

## Why interaction tutorials work <!-- role: reason -->

Many narrative graphics hide useful controls in plain sight. A brief demonstration or visible cue lowers the cost of discovery and helps readers use the intended interaction at the right moment.

**Mechanism:** Tacit tutorials turn interface discovery into part of the narrative, so readers learn controls by watching them used in context.

**Evidence:** The analyzed narratives used animated controls, prompts, and markers of interactivity to teach readers how to navigate and manipulate the display, while a failed case is explicitly attributed in part to dropping readers into the data with little orientation and no tacit tutorial [@segelNarrativeVisualizationTelling2010].

## Use when readers must discover controls inside the story <!-- role: context -->

- **User Goal:** Use interactive controls without stopping to decode the interface.
- **Task:** Learn how to hover, scrub, click, or navigate while following a narrative.
- **Chart Setting:** Interactive stories with lists, buttons, sliders, or other hidden controls.
- **Audience:** First-time or novice readers rather than tool specialists.
- **Success Criterion:** Readers can identify the first meaningful interaction from the interface itself.

## Do not prioritize onboarding over freedom in analyst-first tools <!-- role: exceptions -->

**Break it when:** The display is a reader-driven analysis tool for trained analysts. **Why:** That setting prioritizes immediate free exploration over guided onboarding.

## Costs of interaction tutorials <!-- role: costs -->

**Sacrifice:** Tutorials take narrative time and interface space.\
**Risk:** Instructions feel bolted on if they sit outside the story instead of inside it.\
**Mitigation:** Demonstrate the actual controls as part of the narrative sequence.

## Common failure with interaction tutorials <!-- role: mistakes -->

**Mistake:** Dropping readers directly into the data with no orientation, no example interaction, and no visible signal of what is clickable. **Why it fails:** Useful functionality stays undiscovered and readers miss the intended path into the data.

## How to check interaction tutorials <!-- role: check -->

**Failure Sign:** Important controls are present, but first-time readers have no cue about what to do with them.\
**Quick Check:** Inspect whether each slider, list, or button is either visibly marked as interactive or demonstrated once in the story.\
**Stronger Test:** Ask whether a first-time reader could perform the first intended interaction without outside explanation.

## How to fix undiscoverable interaction <!-- role: fix -->

- Animate the first use of the control inside the narrative sequence.
- Place a short prompt, pointer, or other visible cue next to the interactive control.
- Mark interactive lists, buttons, or sliders so readers can distinguish them from static labels.
