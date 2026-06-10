---
id: change-one-data-dimension-at-a-time-between-consecutive-views
title: Change one data dimension at a time between consecutive visualizations
bibliography: references.bib
description: For linear slideshow-style narrative sequencing, use low-change adjacent
  transitions on multi-view visualization presentations to improve readability and
  mitigate cognitively costly slide-to-slide jumps for audiences following a guided
  presentation.
labels:
- purpose:refine
- basis:empirical
- task:compose
- structure:multi-view
- quality:readability
- lever:layout-structure
---

## Minimize adjacent changes <!-- role: advice -->

Order consecutive visualizations so that each next slide changes as few data attributes as possible, ideally one at a time. For example, keep the independent variable, dependent variable, and level of detail fixed while stepping through time, or insert an intermediate view before jumping across time, measure, and granularity at once.

## Why low-change transitions work <!-- role: reason -->

Small slide-to-slide changes preserve a stable frame for comparison. That makes it easier for viewers to infer why one view follows the next and to connect the sequence into a coherent story.

**Mechanism:** Holding most attributes constant lets viewers compare adjacent views directly instead of re-parsing several new dimensions at once.

**Evidence:** A qualitative analysis of 42 professional narrative visualizations found that local transitions commonly changed only one dimension at a time and suggested maintaining consistency across transitions as a core sequencing principle. In a follow-up user study, participants strongly preferred lower-cost transitions over higher-cost alternatives when choosing which visualization should come next in a presentation [@hullmanDeeperUnderstandingSequence2013].

**Notes:** The paper notes that nearly identical sequences can feel boring, but introducing new unknowns too quickly risks cognitive overload.

## Use when choosing adjacent slide order <!-- role: context -->

- **User Goal:** Guide an audience through a linear data story.
- **Task:** Choose which visualization should appear directly after the current one.
- **Data:** Candidate views differ in independent variable, dependent variable, time, or level of granularity.
- **Chart Setting:** Explicitly guided slideshows, animated data videos, or other linear multi-view presentations.
- **Audience:** Viewers following a guided presentation.
- **Success Criterion:** Viewers can follow the connection between consecutive views without confusion.

## Do not rely on an abrupt multi-change jump when staging is available <!-- role: exceptions -->

**Break it when:** Several aspects of the representation must change and the presentation can stage that change with partial animation. **Why:** The paper observed partial animation being used when multiple aspects changed, as a way to ease transition comprehension.

## Costs of minimizing adjacent changes <!-- role: costs -->

**Sacrifice:** The sequence can advance more slowly because fewer new things change per step.\
**Risk:** A run of very similar visualizations can feel repetitive.\
**Mitigation:** When a larger jump is unavoidable, stage the change instead of switching all attributes at once.

## Common adjacent-change mistake <!-- role: mistakes -->

**Mistake:** Change measure, grouping, time, and detail level all at once between two consecutive views. **Why it fails:** The transition becomes harder to interpret because viewers must infer several differences at the same time.

## Check adjacent transition cost <!-- role: check -->

**Failure Sign:** A viewer struggles to explain why slide B follows slide A.\
**Quick Check:** For each adjacent pair, count how many of these attributes change: independent variable, dependent variable, time, and granularity.\
**Stronger Test:** Compare the current ordering to a reordered version with fewer changes per step and ask viewers which next slide fits better directly after the current one.

## Fix high-cost transitions <!-- role: fix -->

- Reorder slides so adjacent views differ on only one of time, measure, dimension, or granularity.
- Insert an intermediate visualization that holds three attributes constant while changing one.
- Stage an unavoidable multi-attribute jump with partial animation instead of one abrupt switch.
