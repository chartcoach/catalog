---
id: use-table-instead-of-line-chart-for-exact-lookup
title: Use a table instead of a line chart for exact value lookup
bibliography: references.bib
description: For exact lookup tasks on ordered quantitative data, prefer a table over
  a line chart to improve fidelity and mitigate unnecessary visual inference for viewers
  retrieving specific values.
labels:
- purpose:select
- basis:empirical
- task:retrieve
- reading-mode:exact
- chart:table:use
- chart:line:avoid
- quality:fidelity:use
- lever:chart-family
---

## Chart family for exact lookup <!-- role: advice -->

Use a table instead of a line chart when readers must report specific values for named items or periods. For example, list each series value in labeled cells when the task asks for the amount in a particular month, rather than making readers estimate from plotted positions.

## Why a table fits lookup better <!-- role: reason -->

Exact retrieval is a symbolic task. A table presents the requested numbers directly, while a line chart asks readers to read off position and translate it back into a value.

**Mechanism:** A table reduces the need for visual interpolation and supports direct lookup of exact entries.

**Evidence:** The review reports that tables fit textual or symbolic retrieval tasks better than graphs, whereas graphs fit spatial comparison better, showing that chart choice should match the task [@padillaDecisionMakingVisualizations2018].

## Use when the task is direct retrieval <!-- role: context -->

- **User Goal:** Retrieve a specific value accurately.
- **Task:** Report exact numbers for named items, categories, or periods.
- **Data:** Quantitative values with clear row and column identities.
- **Chart Setting:** A choice between a line chart and a table for the same ordered data.
- **Audience:** Readers need exact values rather than overall pattern.
- **Success Criterion:** Fast and accurate lookup without estimation.

## Do not use when the task is pattern comparison <!-- role: exceptions -->

**Break it when:** Readers mainly need to compare differences, ranks, or trends across the ordered sequence. **Why:** Those tasks are easier in a line chart than in a table.

## Costs of choosing the table <!-- role: costs -->

**Sacrifice:** The overall pattern becomes less immediately visible.
**Risk:** Readers may miss trends or relative gaps across many rows and columns.
**Mitigation:** Use this form only when exact lookup is the primary job of the display.

## Common lookup mismatch <!-- role: mistakes -->

**Mistake:** Keep a line chart when the reader's main question is the exact value at a named point. **Why it fails:** The reader must estimate from the axis instead of reading the value directly.

## How to test the chart choice <!-- role: check -->

**Failure Sign:** Reviewers point at the plot and guess, or repeatedly trace from marks to axes to recover a number.
**Quick Check:** Put the same data in a table and a line chart, then ask for an exact named value; choose the form that yields the faster correct answer.
**Stronger Test:** Time a small A/B lookup task with representative readers.

## How to switch to the better form <!-- role: fix -->

- Replace the line chart with a table when the main question is exact value retrieval.
- Put the identifying categories or periods in clear row and column headers.
- Present the values directly in cells instead of requiring axis-based estimation.
