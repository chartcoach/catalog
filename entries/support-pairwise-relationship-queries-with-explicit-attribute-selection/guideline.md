---
id: support-pairwise-relationship-queries-with-explicit-attribute-selection
title: Support pairwise relationship queries with explicit attribute selection
bibliography: references.bib
description: For pairwise relationship analysis of tabular data, use interaction support
  for explicit attribute selection in an information visualization system to improve
  insight and address underspecified correlation questions for analysts.
labels:
- purpose:refine
- basis:empirical
- task:relate
- data:tabular
- quality:insight
- lever:interaction-access
- audience:analyst
---

## Add pairwise relationship controls <!-- role: advice -->

Let viewers choose two attributes and inspect their relationship over the current set of cases. For example, support numeric associations, category-to-attribute coincidences, and trends where time is one of the selected variables.

## Why explicit attribute pairs matter <!-- role: reason -->

Low-level correlation questions are usually about a specified pair of attributes over a specified set of cases. That framing keeps the task concrete, including trend questions where one of the attributes is time.

**Mechanism:** Explicit pair selection turns a vague search for “something related” into a concrete relationship query that the visualization can answer directly.

**Evidence:** Correlate is defined as determining the relationship between two attributes over a given set of data cases, the taxonomy observes that users frequently asked for both numeric and non-numeric correlations, and it interprets trend questions as correlations with temporal variables [@amarLowlevelComponentsAnalytic2005a].

## Use when the relationship is specified <!-- role: context -->

- **User Goal:** Determine whether two chosen attributes relate in a useful way.
- **Task:** Correlate a specified attribute pair over a set of cases.
- **Data:** Tabular data with at least two attributes, including temporal attributes when the question is about trend.
- **Chart Setting:** An information visualization system that can operate on the current subset of cases.
- **Audience:** Analysts asking concrete pairwise relationship questions.
- **Success Criterion:** The system supports direct inspection of the chosen pair, including time paired with another variable when needed.

## Do not use this control for open-ended discovery <!-- role: exceptions -->

**Break it when:** The question is open-ended about any related variable or relies on uncertain criteria. **Why:** Those are higher-level exploratory questions that the primitive correlate task does not directly cover.

## Tradeoffs of explicit pair selection <!-- role: costs -->

**Sacrifice:** The user must specify the two attributes of interest before the system can answer the query.\
**Risk:** Open-ended questions such as “what relates to X?” remain unanswered by this low-level control.\
**Mitigation:** Use the pairwise control for specified questions and keep broader relationship discovery as a separate workflow.

## Common failure modes <!-- role: mistakes -->

**Mistake:** Treating open-ended relationship hunting as the same task as a specified pairwise correlation. **Why it fails:** The low-level task requires a given set of cases and two chosen attributes.

## How to test pairwise relationship support <!-- role: check -->

**Failure Sign:** Users cannot directly specify two attributes and inspect their relation on the current subset.\
**Quick Check:** Choose two attributes and ask for their relationship on a selected set of cases.\
**Stronger Test:** Repeat the check with time as one of the two attributes to confirm support for trend questions.

## What to change <!-- role: fix -->

- Add explicit two-attribute selection for relationship queries.
- Let the pairwise relationship operation run on filtered or otherwise selected subsets.
- Include temporal attributes in the same pairwise relationship control.
