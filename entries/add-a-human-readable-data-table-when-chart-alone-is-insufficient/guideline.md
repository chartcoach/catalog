---
id: add-a-human-readable-data-table-when-chart-alone-is-insufficient
title: Add a human-readable data table when the chart alone does not convey all relevant
  information
bibliography: references.bib
description: For exact reading of chart values, use a companion human-readable data
  table on charts whose title, summary, context, or annotations do not already convey
  all relevant information to improve accessibility and mitigate chart-only presentations
  for users who need different ways to consume information.
labels:
- purpose:refine
- basis:accessibility
- chart:table:use
- structure:multi-view:use
- quality:accessibility
- lever:layout-structure
- reading-mode:exact
---

## Add a companion data table <!-- role: advice -->

Add a human-readable data table alongside the chart when readers need information that the chart title, summary, context, or annotations do not already fully convey. For example, pair a line chart with a table listing the datapoints, and keep the chart as well because the table does not replace the chart's narrative or structural relationships.

## Why a companion data table works <!-- role: reason -->

A chart and a table expose different parts of the same information. The chart carries the higher-level pattern and relationships, while the table exposes the underlying values in a form that can be read directly.

**Mechanism:** A companion table gives readers access to low-level data without forcing the chart to do all exact-value work, and the chart remains available for the broader narrative that a table does not provide.

**Evidence:** Chartability marks the absence of a table as a critical accessibility failure and illustrates that a chart-table pairing can provide low-level datapoint access while preserving the chart's higher-level reading; the linked NCAM guidance also recommends including data tables where appropriate for complex visuals. [@elavskyHowAccessibleMy2022; @wgbh_effective_practices_2]

## Use when chart details are not otherwise available <!-- role: context -->

- **User Goal:** Access the underlying values as well as the chart's overall takeaway.
- **Task:** Read individual datapoints or inspect the data the chart is based on.
- **Data:** The chart contains relevant information not fully conveyed by the existing title, summary, context, or annotations.
- **Chart Setting:** A chart is already present and can be paired with a companion table.
- **Audience:** Readers who use assistive technologies or otherwise prefer a different information flow.
- **Success Criterion:** Readers can access both the high-level chart narrative and the low-level data values.

## Skip the table only when the chart already conveys everything relevant <!-- role: exceptions -->

**Break it when:** The chart title, summary, context, or annotations already convey all relevant information contained in the chart. **Why:** The source explicitly allows the table to be excluded in that case.

## Tradeoffs of a companion data table <!-- role: costs -->

**Sacrifice:** A companion table is an added representation, not a shortcut that removes the need to keep the chart accessible.
**Risk:** Treating the table as a full substitute can remove the narrative and structural relationships that the chart communicates.
**Mitigation:** Keep both the chart and the table available, using the table for low-level values and the chart for higher-level structure.

## Common table fallback mistake <!-- role: mistakes -->

**Mistake:** Replacing the chart with a table and treating the two as equivalent experiences. **Why it fails:** A table may expose the data, but it does not provide an equivalent narrative and may not preserve relationships or interactions that are non-tabular.

## Check for missing value access <!-- role: check -->

**Failure Sign:** The chart shows values or relationships, but no companion human-readable table is available.
**Quick Check:** Ask whether a reader can get all relevant information from the chart title, summary, context, or annotations alone.
**Stronger Test:** Verify that the chart has a companion table containing the data it is based on and that the chart remains available for the higher-level reading.

## Fix missing table access <!-- role: fix -->

- Add a companion human-readable table that contains the data the chart is based on.
- Keep the chart and the table together so readers can use the chart for the overall pattern and the table for exact values.
- If a table is unnecessary because the chart already communicates everything relevant, revise the title, summary, context, or annotations until they convey all relevant information contained in the chart.
