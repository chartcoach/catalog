---
id: insert-a-gap-between-compared-segments-in-a-single-stacked-bar
title: Insert a gap between compared segments in a single stacked bar
bibliography: references.bib
description: For exact part comparison tasks, use visible separation on single stacked
  bars to improve fidelity and mitigate part-to-whole bias for viewers making quick
  visual estimates.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:bar
- quality:fidelity:use
- lever:layout-structure
- operator:part-whole
- reading-mode:exact
---

## Segment spacing inside a stack <!-- role: advice -->

Insert a visible gap between bar segments that readers must compare within one stack. For example, separate the target segments with a gap or other spacing cue instead of leaving them immediately adjacent when viewers must compare one segment's height to another.

## Why a gap works <!-- role: reason -->

Touching segments inside one stack invite a part-to-whole reading that pulls estimates downward. Separating the target segments weakens that whole-bar cue and reduces the bias.

**Mechanism:** A gap shifts the read from “part of one whole” toward “two lengths to compare,” which lowers the negative bias seen with adjacent segments.

**Evidence:** In divided-bar comparisons, immediately adjacent target segments produced high error and strong negative bias, while separating the compared segments reduced error and attenuated the bias; the review includes this paper as evidence on bar-chart variant performance [@talbotFourExperimentsPerception2014; @zengReviewCollationGraphical2023].

## When to use segment spacing <!-- role: context -->

- **User Goal:** Compare two parts inside the same whole exactly.
- **Task:** Judge one stacked segment relative to another segment in the same bar.
- **Data:** Quantitative parts shown inside a single stacked or divided bar.
- **Chart Setting:** The comparison happens within one stack, and the reader could confuse part-to-part with part-to-whole.
- **Audience:** Viewers making quick visual estimates.
- **Success Criterion:** Lower bias and lower absolute error for the target comparison.

## When not to use segment spacing <!-- role: exceptions -->

**Break it when:** The compared values are separate bars in a simple bar chart. **Why:** In simple bar charts, adding separation makes comparison harder rather than easier.

## Tradeoffs of segment spacing <!-- role: costs -->

**Sacrifice:** Some of the immediate continuous-whole appearance of the stack.\
**Risk:** If the whole composition is the only message, extra spacing can weaken that part-to-whole cue.\
**Mitigation:** Use the gap when part-to-part comparison is the priority.

## Common stacked-bar mistake <!-- role: mistakes -->

**Mistake:** Leaving the compared segments touching because they belong to the same whole. **Why it fails:** Adjacency encourages a part-to-whole interpretation and biases the comparison.

## Check for part-to-whole bias <!-- role: check -->

**Failure Sign:** Readers systematically underestimate the smaller segment when the two target segments touch.\
**Quick Check:** Compare an adjacent version with a gapped version and inspect whether the target ratio looks less like a part-of-total judgment.\
**Stronger Test:** Run an A/B estimate task on adjacent versus separated segments and compare bias as well as absolute error.

## Fix adjacent segment bias <!-- role: fix -->

- Add a small gap between the compared segments inside the stack.
- If a gap is not possible, avoid making the touching within-stack segment comparison the primary readout.
- When layout can change, separate the target segments instead of keeping them immediately adjacent.
