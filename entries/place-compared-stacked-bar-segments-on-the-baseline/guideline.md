---
id: place-compared-stacked-bar-segments-on-the-baseline
title: Place compared stacked-bar segments on the baseline
bibliography: references.bib
description: For compare tasks, prefer baseline-aligned segment placement on stacked
  bar charts to improve fidelity and mitigate top-of-stack length judgments for readers
  ranking quantitative parts.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:bar
- quality:fidelity:use
- lever:layout-structure
- channel:position:use
---

## Segment order in stacked bars <!-- role: advice -->

Put the segment readers need to compare at the bottom of each stack so both values share the baseline. For example, compare two bottom segments rather than two top segments or one segment placed above another when readers must judge which segment is larger.

## Why bottom segments work better <!-- role: reason -->

Baseline alignment changes the read from floating length estimation to position on a common scale. Bottom segments share that scale, while top segments force readers to judge lengths detached from the baseline.

**Mechanism:** Shared-baseline segments support more accurate ranking because both compared values start from the same reference line.

**Evidence:** In the reported sort experiment, the bottom-of-stack condition ranked above the top-of-stack conditions, and the pairwise differences against the two top-segment variants were significant; the collated record also shows that an adjacent-bar version ranked highest overall in the same comparison family [@zengReviewCollationGraphical2023; @clevelandGraphicalPerceptionTheory1984].

## Use when a stacked bar chart is already fixed <!-- role: context -->

- **User Goal:** Compare the size of one segment across bars.
- **Task:** Rank quantitative segments accurately.
- **Data:** Quantitative parts displayed within stacked totals.
- **Chart Setting:** A stacked bar chart is already chosen or required.
- **Audience:** Readers making quick visual judgments.
- **Success Criterion:** More accurate segment ordering inside the stacked layout.

## Do not use when you can remove the stack <!-- role: exceptions -->

**Break it when:** You can unstack the compared values into ordinary adjacent bars on the same scale. **Why:** The adjacent-bar condition ranked above every stacked-bar condition in the experiment.

## What this refinement cannot solve <!-- role: costs -->

**Sacrifice:** Only one segment can occupy the baseline in each stack.
**Risk:** Other cross-segment comparisons in the same stack remain hard.
**Mitigation:** Split the stack into adjacent bars when several segment-to-segment comparisons matter.

## Common stacked-bar mistake <!-- role: mistakes -->

**Mistake:** Leaving the compared segments at the top of the stacks or placing one compared value above another. **Why it fails:** That turns the task back into length judgments without a shared baseline and performed worse in the experiment.

## How to check the segment placement <!-- role: check -->

**Failure Sign:** The compared segments do not start from the same baseline.
**Quick Check:** Trace the bottoms of the two compared segments to see whether both touch the zero line.
**Stronger Test:** Make a second version with the compared segment moved to the bottom, or unstacked into adjacent bars, and compare which version makes the ordering easier to judge.

## What to change <!-- role: fix -->

- Reorder the stack so the compared segment starts at the baseline.
- If two compared segments cannot both share the baseline inside one stack, split them into adjacent bars.
- Use the ordinary adjacent-bar layout when the chart must support several accurate segment comparisons.
