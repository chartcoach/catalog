---
id: identify-anomalies-separately-from-extreme-values
title: Identify anomalies separately from extreme values
bibliography: references.bib
description: For record-list exception analysis of quantitative data, use interaction
  support for anomaly identification in an information visualization system to improve
  insight and address the mistake of treating anomalies as maxima or minima for analysts.
labels:
- purpose:refine
- basis:empirical
- scope:record-list
- data:quantitative
- shape:outlier-rich
- quality:insight
- lever:interaction-access
- audience:analyst
---

## Add an anomaly operation <!-- role: advice -->

Provide a dedicated anomaly operation that flags exceptional cases against a relationship or distribution. For example, isolate outliers in a numeric attribute or exceptions to an expected two-attribute relation even when those cases are not the absolute highest or lowest values.

## Why anomalies need their own operation <!-- role: reason -->

Exceptional cases often drive follow-up analysis, but they are not the same as the largest or smallest cases. An anomaly is defined against an expectation, a relationship, or a distribution.

**Mechanism:** Separate anomaly support helps viewers find exceptions to what looks normal, instead of collapsing exception finding into simple ranking.

**Evidence:** Find Anomalies is defined as identifying unexpected or exceptional values with respect to a relationship or expectation, and the taxonomy explicitly distinguishes anomalies from extrema by noting that anomalies are not always extreme values [@amarLowlevelComponentsAnalytic2005a].

## Use when the question is about exceptions <!-- role: context -->

- **User Goal:** Find outliers or exceptions to an expected pattern.
- **Task:** Identify anomalous cases within a selected set.
- **Data:** Quantitative attributes or quantitative relationships where exceptions can occur.
- **Chart Setting:** An information visualization system that already supports selecting a set of cases or specifying a relation of interest.
- **Audience:** Analysts using anomalies as a basis for further exploration.
- **Success Criterion:** The system surfaces exceptional cases without reducing the task to top/bottom ranking.

## Do not use anomaly detection for simple ranking <!-- role: exceptions -->

**Break it when:** The user needs the highest or lowest N cases by an attribute. **Why:** That is an extremum task, not an anomaly task.

## Tradeoffs of a separate anomaly operation <!-- role: costs -->

**Sacrifice:** The output prioritizes exceptional cases instead of a complete ranking.\
**Risk:** Treating every large or small value as anomalous produces false exception hunts.\
**Mitigation:** Define anomalies against a relationship or a distribution, not just against absolute size.

## Common failure modes <!-- role: mistakes -->

**Mistake:** Equating outlier detection with top/bottom ranking. **Why it fails:** An anomalous case may be exceptional relative to a pattern without being the global maximum or minimum.

## How to test anomaly support <!-- role: check -->

**Failure Sign:** The only way to look for outliers is to sort ascending or descending.\
**Quick Check:** Ask for outliers in one attribute and for exceptions to a two-attribute relation.\
**Stronger Test:** Verify that the system can surface both kinds of anomalies without relying on global max/min lists.

## What to change <!-- role: fix -->

- Add anomaly detection against the current distribution of one attribute.
- Add anomaly detection against the current relationship between two attributes.
- Keep anomaly controls separate from top/bottom ranking controls.
