---
id: provide-aggregate-calculations-over-selected-cases
title: Provide aggregate calculations over selected cases
bibliography: references.bib
description: For grouped-result analysis of tabular data, use interaction support
  for aggregate calculations on subsets in an information visualization system to
  improve insight and address comparisons that depend on summary values for analysts.
labels:
- purpose:refine
- basis:empirical
- task:compose
- scope:grouped-result
- data:tabular
- quality:insight
- lever:interaction-access
- audience:analyst
---

## Expose aggregate functions <!-- role: advice -->

Add aggregate functions that operate on the current set of cases. For example, let viewers compute average, sum, count, or count-unique-values over a filtered subset instead of inferring group comparisons from raw records alone.

## Why aggregate functions need direct support <!-- role: reason -->

Many analytic questions are really about a numeric summary of a set, not about any one record. Direct aggregate support turns a subset into a concrete value that can be read and compared.

**Mechanism:** Aggregate functions convert a selected set of cases into an explicit numeric result, which makes vague group comparisons answerable and keeps the calculation inside the visualization workflow.

**Evidence:** Compute Derived Value is defined as computing an aggregate numeric representation over a set of data cases, and the taxonomy notes that many comparison questions imply an aggregation function even when the question does not specify exactly how the comparison should be calculated [@amarLowlevelComponentsAnalytic2005a].

## Use when the answer is a summary, not a raw record <!-- role: context -->

- **User Goal:** Summarize a group or compare groups using a numeric summary.
- **Task:** Compute a derived value over a selected set of cases.
- **Data:** Tabular cases that can be grouped or filtered into subsets.
- **Chart Setting:** An information visualization system that already supports selecting a set of cases.
- **Audience:** Analysts asking questions about categories, subsets, or totals.
- **Success Criterion:** The system returns the needed summary value directly on the selected set.

## Do not use aggregate calculations for direct lookup <!-- role: exceptions -->

**Break it when:** The question asks for raw attributes of already specified cases. **Why:** That is a retrieve-value task, not a compute-derived-value task.

## Tradeoffs of explicit aggregation <!-- role: costs -->

**Sacrifice:** The user must choose an aggregation function instead of leaving the comparison vague.\
**Risk:** Different aggregation functions can answer materially different questions.\
**Mitigation:** Make the active aggregation function explicit wherever the derived value appears.

## Common failure modes <!-- role: mistakes -->

**Mistake:** Leaving the comparison metric implicit in questions such as “which group is more X.” **Why it fails:** The question stays underspecified until a concrete aggregation function is chosen.

## How to test aggregate support <!-- role: check -->

**Failure Sign:** Users must calculate averages, totals, or counts outside the visualization.\
**Quick Check:** Ask the system for an average, a sum, and a count-unique over the current subset.\
**Stronger Test:** Try a group comparison that depends on a summary metric and verify that the system exposes which aggregation function produced the answer.

## What to change <!-- role: fix -->

- Add average, sum, count, and count-unique operations.
- Let aggregate functions run on filtered or otherwise selected subsets.
- Show the chosen aggregation function alongside the derived value.
