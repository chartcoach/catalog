---
id: arrange-sequential-panels-in-a-single-row
title: Arrange sequential panels in a single row
bibliography: references.bib
description: For relate tasks in multi-measure temporal panels, use a single-row layout
  on small-multiple line charts to improve sequential readability and mitigate unclear
  reading order for readers being guided through a deliberate story.
labels:
- purpose:refine
- basis:heuristic
- task:relate
- chart:line
- structure:small-multiples
- quality:readability
- lever:layout-structure
- aesthetic:composition:use
---

## Single-row panel layout <!-- role: advice -->

Arrange the panels in a single horizontal row when the chart needs to be read as a sequence. For example, take a four-panel multiple line chart that is arranged as a block and place the panels left to right so they work like a comic strip.

## Why a single row works <!-- role: reason -->

A single row gives readers one obvious path through the chart. That matters when the chart is not meant to be absorbed at a glance but to unfold step by step.

**Mechanism:** A one-row layout reduces ambiguity about where to look next and makes the panel sequence itself carry the reading order.

**Evidence:** The post frames interrelated trend panels as an "unfolding story" and specifically recommends putting the panels in a single row to create a clear linear sequence [@mintzer_sequential_storytelling_2024].

## Use when the chart needs a guided reading path <!-- role: context -->

- **User Goal:** Show how several trends connect to one another.
- **Task:** Guide the reader through the visualization in a deliberate sequence.
- **Data:** Multiple related measures shown in separate panels over time.
- **Chart Setting:** A multiple line chart or other panelled chart already split into several views.
- **Audience:** Readers expected to follow the chart one panel at a time.
- **Success Criterion:** The reading order is obvious from left to right.

## Do not use when the chart should be taken in at a glance <!-- role: exceptions -->

**Break it when:** The chart does not need deliberate sequencing and can be understood at a glance. **Why:** The extra linear scaffold is unnecessary.

## Costs of using one row <!-- role: costs -->

**Sacrifice:** You give up the more compact block arrangement.
**Risk:** A single row can still feel arbitrary if the panel order does not carry the story.
**Mitigation:** Pair the one-row layout with a deliberate panel order.

## Common layout failure <!-- role: mistakes -->

**Mistake:** Keeping sequential panels in a wrapped block while trying to tell a left-to-right story. **Why it fails:** The reader has a weaker cue for where the sequence continues.

## How to test the reading path <!-- role: check -->

**Failure Sign:** Readers hesitate about where to look after the first panel.
**Quick Check:** Compare the current layout with a one-row version and see whether the reading path becomes obvious without extra explanation.
**Stronger Test:** If you still need to tell readers which panel comes next, the layout is not doing enough.

## What to change <!-- role: fix -->

- Move the panels from a block arrangement into one horizontal row.
- Make the sequence begin at the left edge and end at the right edge.
- If the row still feels scrambled, reorder the panels to match the story.
