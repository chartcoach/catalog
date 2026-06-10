---
id: expose-a-distribution-summary-for-quantitative-attributes
title: Expose a distribution summary for quantitative attributes
bibliography: references.bib
description: For grouped-result distribution analysis of quantitative data, use interaction
  support for distribution summaries in an information visualization system to improve
  insight and address judgments about normalcy or case location within a spread for
  analysts.
labels:
- purpose:refine
- basis:empirical
- task:distribute
- scope:grouped-result
- data:quantitative
- quality:insight
- lever:interaction-access
- audience:analyst
---

## Add a distribution view <!-- role: advice -->

Add a distribution summary for a quantitative attribute over the current set of cases. For example, show the spread of calories, ages, or film lengths across a selected set so viewers can judge what is typical and where one case sits within that spread.

## Why distribution matters beyond single values <!-- role: reason -->

A spread tells viewers what is normal in the data and where a case falls relative to that normal pattern. Some seemingly simple comparison questions are actually questions about position within a full distribution.

**Mechanism:** Distribution summaries support judgments about normalcy and relative position that cannot be answered from one exact value or one aggregate alone.

**Evidence:** Characterize Distribution is defined as describing the distribution of a quantitative attribute over a set of cases; the taxonomy states that users use distribution to understand normalcy versus anomaly and notes that some comparison questions are really questions about location within a distribution [@amarLowlevelComponentsAnalytic2005a].

## Use when the user needs spread or typicality <!-- role: context -->

- **User Goal:** Understand what values are typical, how values are spread, or where one case falls relative to others.
- **Task:** Characterize the distribution of a quantitative attribute over a set.
- **Data:** A quantitative attribute measured across multiple cases.
- **Chart Setting:** An information visualization system that can operate on a selected subset of cases.
- **Audience:** Analysts exploring a dataset for structure and normalcy.
- **Success Criterion:** The system reveals the spread of values, not only exact lookups or one-number summaries.

## Do not use a distribution summary for span-only questions <!-- role: exceptions -->

**Break it when:** The user needs only the span of values or the list of unique values. **Why:** That is a range task, not a full distribution task.

## Tradeoffs of a distribution summary <!-- role: costs -->

**Sacrifice:** The output summarizes a set of values rather than returning one exact case value.\
**Risk:** A distribution summary alone may not identify the exceptional cases that motivate follow-up.\
**Mitigation:** Use a separate anomaly operation when the goal is to find exceptions.

## Common failure modes <!-- role: mistakes -->

**Mistake:** Replacing the full spread with only a single average when the real question is “how does this case compare to others.” **Why it fails:** That question is about location within a distribution, not only about the mean.

## How to test distribution support <!-- role: check -->

**Failure Sign:** Reviewers can read individual records or a single aggregate, but not the spread of a quantitative attribute.\
**Quick Check:** Ask for the distribution of one quantitative attribute on a selected subset.\
**Stronger Test:** Select one case and verify that the system can place it relative to the current spread.

## What to change <!-- role: fix -->

- Add a distribution summary that updates on the current set of cases.
- Let viewers inspect where a selected case falls within the current spread.
- Add a separate anomaly operation if the real goal is to identify exceptions.
