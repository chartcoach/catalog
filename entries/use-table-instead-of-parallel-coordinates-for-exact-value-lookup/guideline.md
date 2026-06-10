---
id: use-table-instead-of-parallel-coordinates-for-exact-value-lookup
title: Use a table instead of a parallel coordinates plot for exact value lookup
bibliography: references.bib
description: For exact value-retrieval tasks on small multivariate record sets, prefer
  a table over a parallel coordinates plot to improve fidelity and address slow cross-axis
  tracing for exact-reading situations.
labels:
- purpose:select
- basis:empirical
- task:retrieve
- chart:table:use
- chart:parallel:avoid
- quality:fidelity:use
- lever:chart-family
- measure:multi
---

## Choose the lookup representation <!-- role: advice -->

Use a table when the job is exact cross-attribute value lookup. For example, replace a parallel coordinates plot with a table when readers must locate one record by a shown value and then read another value from the same 4-attribute, 8-record dataset.

## Why a table helps exact lookup <!-- role: reason -->

A table shows the exact values directly in cells, while a parallel coordinates plot makes the reader follow a line from one axis to another before reading the target value.

**Mechanism:** A table preserves a direct row-based lookup path across attributes. This avoids the extra line tracing required in a parallel coordinates plot.

**Evidence:** The collated record ranks the table ahead of the parallel coordinates plot on retrieve-value response time and reports no accuracy difference, matching the original experiment's finding that tables were fastest for value retrieval [@zengReviewCollationGraphical2023; @kanjanaboseMultitaskComparativeStudy2015].

## Use when exact lookup is the job <!-- role: context -->

- **User Goal:** Find one attribute value after locating the same record by another attribute.
- **Task:** Exact value retrieval across attributes.
- **Data:** 8 records with 4 quantitative attributes and record IDs.
- **Chart Setting:** Static representations of the same records and attributes with no interaction.
- **Success Criterion:** Faster correct lookup of exact values.

## Do not use this choice for pattern-finding tasks <!-- role: exceptions -->

**Break it when:** The user goal changes from exact lookup to clustering or anomaly detection. **Why:** In the same study, parallel coordinates plots outperformed the table on those tasks.

## Tradeoffs of replacing a parallel coordinates plot with a table <!-- role: costs -->

**Sacrifice:** You give up the stronger visual support for multivariate pattern finding.
**Risk:** Keeping the parallel coordinates plot for lookup adds tracing work without improving correctness.
**Mitigation:** Use the table for exact lookup and reserve the plot for pattern-detection tasks.

## Common lookup failure <!-- role: mistakes -->

**Mistake:** Keeping a parallel coordinates plot for exact cross-attribute lookup. **Why it fails:** Readers must trace a line across axes, which was slower than reading the table directly.

## Check the lookup choice <!-- role: check -->

**Failure Sign:** Reviewers follow polylines across axes before they can answer a simple lookup question.
**Quick Check:** Show the same lookup prompt in a table and in a parallel coordinates plot, and compare whether the table gets the same correct answer faster.
**Stronger Test:** Repeat several exact lookup prompts on matched table and parallel versions and compare average completion time.

## Fix the lookup view <!-- role: fix -->

- Replace the parallel coordinates plot with a table for exact value-retrieval prompts.
- Present the same records and attributes as cells when the answer is a single exact value.
- Switch back to a visual representation only when the task changes from lookup to clustering or anomaly detection.
