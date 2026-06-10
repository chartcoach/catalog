---
id: encode-differences-as-visual-objects
title: Encode pairwise differences as visual objects when comparison is the task
bibliography: references.bib
description: For comparison across many paired values, use direct difference encoding
  on grouped charts to improve insight and mitigate slow one-by-one comparison for
  readers scanning multiple pairs.
labels:
- purpose:refine
- basis:empirical
- task:compare
- quality:insight:use
- lever:encoding
- operator:difference
- measure:multi
- density:dense
---

## Show the delta directly <!-- role: advice -->

Turn each pairwise difference into its own mark instead of forcing readers to compare two marks repeatedly. For example, replace repeated before/after bar pairs with a single positive or negative difference bar so increasing and decreasing cases become visible immediately.

## Why direct deltas work <!-- role: reason -->

Readers can rapidly find a maximum or summary pattern in a display, but pairwise comparison slows down because it is performed one relation at a time. A direct delta turns the relation itself into something the eye can see as an object.

**Mechanism:** Direct difference encoding removes repeated pairwise comparison steps, so readers can spot the relation of interest without scanning every pair serially.

**Evidence:** The paper states that comparison is unusually slow relative to other visual operations, illustrates this with a paired-bar example, and shows that turning differences into visual objects makes the comparison task simpler [@zacksDesigningGraphsDecisionMakers2020].

## Use when many pairs must be compared <!-- role: context -->

- **User Goal:** Find which pairs increase, decrease, or differ most.
- **Task:** Compare many paired values.
- **Data:** Paired quantitative values across multiple items.
- **Chart Setting:** The current design uses repeated left/right or before/after mark pairs.
- **Audience:** Readers who do not know in advance which pair matters.
- **Success Criterion:** Readers can identify the relevant pair or direction quickly.

## Do not use when a single-value summary is the goal <!-- role: exceptions -->

**Break it when:** The goal is simply to find the highest single value or another collection summary. **Why:** Standard position-based displays already support those tasks efficiently.

## Make the comparison primary <!-- role: costs -->

**Sacrifice:** The original pair members become less visually primary than the difference itself.
**Risk:** If the original paired marks still dominate the display, the comparison bottleneck remains.
**Mitigation:** Make the delta mark the primary object when the message is the difference.

## Avoid leaving the relation implicit <!-- role: mistakes -->

**Mistake:** Keeping two full marks for each pair and expecting viewers to spot the special relation at a glance. **Why it fails:** Readers still have to compare the marks one pair at a time.

## Check whether comparison is still serial <!-- role: check -->

**Failure Sign:** Readers inspect nearly every pair before answering.
**Quick Check:** Ask someone to find the unique decreasing pair; if they scan pair by pair, the difference is not directly encoded.
**Stronger Test:** Compare the paired-value version with a delta-encoded version on the same question and keep the version that makes the answer more immediate.

## Turn relations into marks <!-- role: fix -->

- Replace paired bars or points with a single difference mark.
- Encode the sign or direction of the difference so increases and decreases are visually distinct.
- Remove or de-emphasize redundant paired marks when the difference is the message.
