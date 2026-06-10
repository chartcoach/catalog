---
id: use-table-instead-of-scatter-for-exact-value-lookup
title: Use a table instead of a scatter plot for exact value lookup
bibliography: references.bib
description: For exact value-retrieval tasks on small multivariate record sets, prefer
  a table over a scatter plot to improve fidelity and address slow cross-attribute
  lookup for exact-reading situations.
labels:
- purpose:select
- basis:empirical
- task:retrieve
- chart:table:use
- chart:scatter:avoid
- quality:fidelity:use
- lever:chart-family
- measure:multi
---

## Choose the lookup representation <!-- role: advice -->

Use a table when the job is exact cross-attribute value lookup. For example, replace a scatter plot view with a table when readers must find a record from one shown value and then read a second value from the same 4-attribute, 8-record dataset.

## Why a table helps exact lookup <!-- role: reason -->

A table supports direct scanning of rows and columns for an exact answer, while a scatter plot view makes the reader trace points across attributes before reading the target value.

**Mechanism:** A table keeps the lookup path explicit: find the record, stay on the same row, and read the target cell. This reduces the extra tracing needed in a scatter plot view.

**Evidence:** The collated record ranks the table ahead of the scatter plot on retrieve-value response time and reports no accuracy difference, matching the original experiment's conclusion that tables were fastest for value retrieval while scatter plots were slowest [@zengReviewCollationGraphical2023; @kanjanaboseMultitaskComparativeStudy2015].

## Use when exact lookup is the job <!-- role: context -->

- **User Goal:** Find one attribute value after locating the same record by another attribute.
- **Task:** Exact value retrieval across attributes.
- **Data:** 8 records with 4 quantitative attributes and record IDs.
- **Chart Setting:** Static representations of the same records and attributes with no interaction.
- **Success Criterion:** Faster correct lookup of exact values.

## Do not use this choice for pattern-finding tasks <!-- role: exceptions -->

**Break it when:** The user goal changes from exact lookup to clustering or anomaly detection. **Why:** In the same study, the table was not the best-performing representation for those pattern-finding tasks.

## Tradeoffs of replacing a scatter plot with a table <!-- role: costs -->

**Sacrifice:** You give up the stronger visual support for multivariate pattern finding.
**Risk:** Keeping the scatter plot for lookup slows readers without improving correctness.
**Mitigation:** Switch back to a visual representation when the task changes from lookup to pattern detection.

## Common lookup failure <!-- role: mistakes -->

**Mistake:** Keeping a scatter plot view for exact cross-attribute lookup. **Why it fails:** Readers must trace marks across attributes, which was slower than reading the table directly.

## Check the lookup choice <!-- role: check -->

**Failure Sign:** Reviewers hesitate while tracing points before answering a lookup question.
**Quick Check:** Show the same lookup prompt in a table and in a scatter plot view, and compare whether the table gets the same correct answer faster.
**Stronger Test:** Repeat several exact lookup prompts on matched table and scatter versions and compare average completion time.

## Fix the lookup view <!-- role: fix -->

- Replace the scatter plot view with a table for exact value-retrieval prompts.
- Present the same records and attributes as cells when the answer is a single exact value.
- Switch back to a visual representation only when the task changes from lookup to clustering or anomaly detection.
