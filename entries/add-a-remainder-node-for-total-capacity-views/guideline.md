---
id: add-a-remainder-node-for-total-capacity-views
title: Add a remainder node when the treemap must represent the full available total
bibliography: references.bib
description: For utilization overview of a hierarchical total, use a remainder node
  at the treemap root to improve fidelity and address displays that omit unused capacity
  for users reading percentage of total use.
labels:
- purpose:refine
- basis:empirical
- chart:treemap
- data:hierarchical
- quality:fidelity
- lever:encoding
- operator:part-whole
---

## Add a remainder node <!-- role: advice -->

Add one extra child at the treemap root to represent the unused remainder when the display must show percentage of total capacity rather than only the used hierarchy. For example, include a rectangle for unused space so the root covers both the used leaves and the unallocated remainder.

## Why the remainder node works <!-- role: reason -->

A treemap can show only the used hierarchy unless the unused part is added explicitly. Adding a remainder node makes the root correspond to the full available total instead of only the used portion.

**Mechanism:** The extra child closes the part-whole accounting at the root, so area can be interpreted as percentage of the full available total.

**Evidence:** The paper states that if users want the display as a percentage of total utilization, the root must have one additional dummy child whose size is the entire unused portion [@shneidermanTreeVisualizationTreemaps1992].

## Use when the root must mean the full total <!-- role: context -->

- **User Goal:** Read the treemap as percentage of the full available total.
- **Task:** Part-whole interpretation of used versus unused capacity.
- **Data:** A used hierarchy plus an unused remainder.
- **Chart Setting:** A treemap rooted at the full resource being monitored.
- **Audience:** Users monitoring overall utilization.
- **Success Criterion:** The sum of the root's children equals the full available total.

## Do not use when only the used hierarchy should be shown <!-- role: exceptions -->

**Break it when:** The display is intended to show only the used hierarchy rather than percentage of total capacity. **Why:** The paper adds the dummy child specifically for the percentage-of-total interpretation.

## Costs of adding the remainder node <!-- role: costs -->

**Sacrifice:** Some of the display area is assigned to the unused remainder instead of to used nodes.
**Risk:** A large remainder can compress the visible area of the used hierarchy.
**Mitigation:** Add the remainder only when percentage of total capacity is the intended reading.

## Common failure mode in this refinement <!-- role: mistakes -->

**Mistake:** Presenting a used-only treemap as if it showed percentage of the full total. **Why it fails:** The root no longer includes the unused portion, so the part-whole reading is incomplete.

## How to test the total-capacity encoding <!-- role: check -->

**Failure Sign:** The root represents only the used hierarchy even though the view is labeled or read as total utilization.
**Quick Check:** Sum the root's children and verify that they equal used plus unused capacity.
**Stronger Test:** Compare the used-only treemap with the version that includes the remainder node and confirm that only the latter supports a percentage-of-total reading.

## What to change <!-- role: fix -->

- Compute the unused remainder at the root.
- Add one dummy child for that unused amount.
- Size the dummy child by the full unused portion.
- Distinguish the remainder in the treemap so the root now represents the complete total.
