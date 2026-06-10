---
id: add-a-visible-progress-tracker-for-multi-step-narratives
title: Add a visible progress tracker for multi-step narratives
bibliography: references.bib
description: For ordered narrative walkthroughs, use a progress tracker on multi-frame
  presentations to improve readability and mitigate loss of place for readers moving
  through sequential sections.
labels:
- purpose:refine
- basis:empirical
- structure:multi-view
- quality:readability:use
- lever:layout-structure
- communication:workflow
---

## Progress and location cues <!-- role: advice -->

Add a visible progress tracker that shows both the current step and the full length of the narrative. For example, place a progress bar above a slideshow, use a timebar that updates with the chart, or mirror the sections in a checklist overview that readers can also use for navigation.

## Why progress cues work <!-- role: reason -->

Narrative graphics ask readers to manage both content and sequence. A visible tracker tells readers where they are, how much remains, and where they can jump next without breaking orientation.

**Mechanism:** Progress cues externalize narrative structure, so readers do not have to infer sequence and location from changing content alone.

**Evidence:** The analyzed slide-based narratives used progress bars, timebars, and checklist overviews to communicate structure, preserve orientation, and support navigation, and the paper identifies these as recurring visual-structuring tactics [@segelNarrativeVisualizationTelling2010].

## Use when the story has an ordered sequence <!-- role: context -->

- **User Goal:** Move through a multi-step explanation while knowing current position and remaining steps.
- **Task:** Follow a sequence of authored sections or slides.
- **Chart Setting:** Multi-frame presentations with next/back controls or section tabs.
- **Audience:** Readers who need help tracking narrative order.
- **Success Criterion:** Readers can tell where they are and how far the story goes at any step.

## Do not add sequence trackers to unordered views <!-- role: exceptions -->

**Break it when:** The graphic is a single-frame view or an intentionally random-access exploratory display with no prescribed order. **Why:** There is no narrative path to track.

## Costs of progress cues <!-- role: costs -->

**Sacrifice:** Progress trackers consume visible space.\
**Risk:** A tracker that does not match the actual sequence misleads readers about where they are.\
**Mitigation:** Keep the tracker synchronized with the real section order and, when possible, make it navigable.

## Common failure with progress cues <!-- role: mistakes -->

**Mistake:** Hiding sequence in next/back controls alone without showing total length or current position. **Why it fails:** Readers cannot tell where they are in the story or how the current step relates to the whole.

## How to check progress cues <!-- role: check -->

**Failure Sign:** Readers can advance, but cannot tell current section or remaining length from the interface.\
**Quick Check:** At any frame, verify that the current step and total number of steps are visible.\
**Stronger Test:** Step through the sequence and confirm that the progress indicator updates in sync with each frame.

## How to fix missing progress cues <!-- role: fix -->

- Add a progress bar or timebar that marks current position and total span.
- Mirror the section structure in a checklist or overview screen when the narrative has named segments.
- Make the tracker itself a navigation device when the interface supports jumping between sections.
