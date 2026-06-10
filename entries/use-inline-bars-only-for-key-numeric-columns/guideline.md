---
id: use-inline-bars-only-for-key-numeric-columns
title: Use inline bars only for the most important numeric columns
bibliography: references.bib
description: For multi-measure tables with numeric columns, use inline bars on the
  most important table columns to improve overview and mitigate overly wide quantitative
  columns for readers who still need exact values.
labels:
- purpose:refine
- basis:heuristic
- chart:table
- data:quantitative
- quality:insight
- lever:encoding
- measure:multi
- channel:length:use
---

## Inline bars in key columns <!-- role: advice -->

Add inline bar charts to the most important numeric columns in a table. For example, use bars for one or a few key measures while keeping exact numbers readable, and do not turn every numeric column into a bar column.

## Why selective inline bars help <!-- role: reason -->

Inline bars can add an at-a-glance overview without giving up exact table values.

**Mechanism:** Bars reveal relative size quickly, but each bar column needs more width than a plain number column, so selectivity keeps the table readable.

**Evidence:** The post says bar charts can combine the readability and sortability of tables with the quick overview of charts, but warns that bar columns are often wider than normal number columns and should be used only for the most important column or columns [@muth_tables_2019].

## Use when exact values and overview both matter <!-- role: context -->

- **User Goal:** Keep exact numbers while also showing relative magnitude quickly.
- **Task:** Read a table with more than one numeric measure.
- **Data:** Quantitative columns inside an already chosen table.
- **Chart Setting:** Table width is limited.
- **Success Criterion:** Readers see the main magnitude pattern without the table becoming too wide.

## Do not use on every numeric column <!-- role: exceptions -->

**Break it when:** Many numeric columns would all need bars. **Why:** The post says bar columns are wider than standard number columns.

## Tradeoffs of inline bars <!-- role: costs -->

**Sacrifice:** You give up some horizontal space.\
**Risk:** Adding bars to every numeric column can make the table too wide.\
**Mitigation:** Limit bars to one or a few key measures and leave secondary measures as numbers.

## Common inline-bar mistake <!-- role: mistakes -->

**Mistake:** Converting every numeric column into a bar column. **Why it fails:** The overview gain is outweighed by a wider, harder-to-read table.

## Check whether the bars are worth the width <!-- role: check -->

**Failure Sign:** Bar columns crowd the table or force other columns to become harder to read.\
**Quick Check:** Remove bars from secondary numeric columns and compare the table width.\
**Stronger Test:** Keep bars only on the one or few measures that still convey the main pattern at a glance.

## Fix the encoding mix <!-- role: fix -->

- Choose the one or few numeric columns that matter most to the story.
- Add inline bars only to those key columns.
- Leave the remaining numeric columns as plain numbers.
