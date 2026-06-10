---
id: separate-threshold-filters-from-top-bottom-queries
title: Separate threshold filters from top/bottom queries
bibliography: references.bib
description: For record-list analysis of tabular data, use distinct interaction controls
  on an information visualization system to improve insight and address confusion
  between concrete conditions and relative rankings for analysts.
labels:
- purpose:refine
- basis:empirical
- scope:record-list
- data:tabular
- quality:insight
- lever:interaction-access
- audience:analyst
---

## Separate threshold and top/bottom controls <!-- role: advice -->

Implement threshold filtering and extremum finding as separate interaction controls. For example, use explicit “greater than x” conditions to return matching cases, and separate top/bottom N actions for highest, lowest, most recent, or most-awarded cases.

## Why the separation matters <!-- role: reason -->

Threshold queries and top/bottom queries are different analytic operations. One tests each case against a concrete condition. The other depends on how every case ranks relative to the full set.

**Mechanism:** Separate controls keep users from confusing an absolute condition with a relative ranking and let the system answer each question directly.

**Evidence:** Filter is defined as finding cases that satisfy concrete conditions independent of other data cases, while Find Extremum is defined as finding top or bottom cases relative to the attribute range in the data set; the taxonomy also notes that vague requests such as “high” become filter questions only after the threshold is made explicit [@amarLowlevelComponentsAnalytic2005a].

## Use when the query is thresholded or top/bottom <!-- role: context -->

- **User Goal:** Find records above or below a concrete cutoff, or identify the highest or lowest records.
- **Task:** Select matching cases or retrieve top/bottom cases from a set.
- **Data:** Tabular cases with attributes that can be thresholded or ranked.
- **Chart Setting:** An information visualization system with interactive case selection.
- **Audience:** Analysts asking specific low-level questions about a dataset.
- **Success Criterion:** The system answers both threshold and top/bottom questions without forcing users to recast one as the other.

## Do not use this split for known-case lookup <!-- role: exceptions -->

**Break it when:** The cases are already known and the job is only to read their attributes. **Why:** That is a retrieve-value task, not a filter or extremum task.

## Tradeoffs of separating the controls <!-- role: costs -->

**Sacrifice:** You give up a single generic “high/low” action that blurs threshold conditions and relative ranking.\
**Risk:** A filter without an explicit cutoff still leaves “high” undefined.\
**Mitigation:** Make filter criteria concrete and keep top/bottom actions explicitly relative to the set.

## Common failure modes <!-- role: mistakes -->

- **Mistake:** Treating “high value” as a filter without defining the cutoff. **Why it fails:** The question is not concrete until the operating definition is made explicit.
- **Mistake:** Using full sorting as the only way to answer a single max/min question. **Why it fails:** Finding an extremum is a different task from ordering the entire set.

## How to test the control split <!-- role: check -->

**Failure Sign:** Users can answer “greater than x” only by ranking everything, or answer “highest” only by guessing a threshold.\
**Quick Check:** Ask the system for both an above-threshold list and a top-1 or top-N list on the same attribute.\
**Stronger Test:** Verify that each query is answered by its own control without manual recoding of the task.

## What to change <!-- role: fix -->

- Add explicit threshold-based filter controls for concrete conditions.
- Add separate top/bottom N controls for relative ranking queries.
- Rename vague “high/low” actions so they resolve to either a numeric threshold or a ranking operation.
