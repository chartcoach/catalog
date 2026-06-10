---
id: use-lining-tabular-numerals-for-chart-values
title: Use lining tabular numerals for chart values
bibliography: references.bib
description: For exact reading of values in charts and tables, use lining tabular
  numerals on labels, axis ticks, tooltips, and table cells to improve readability
  and mitigate misalignment from varying digit heights and widths for readers comparing
  numbers.
labels:
- purpose:refine
- basis:heuristic
- data:quantitative
- quality:readability
- lever:text-annotation
- reading-mode:exact
---

## Align values with lining tabular numerals <!-- role: advice -->

Use lining tabular numerals for quantitative text in charts and tables. For example, keep table cells, tooltip values, and axis ticks in numerals that share the same height and width instead of oldstyle or proportional figures.

## Why lining tabular numerals work <!-- role: reason -->

Readers compare numeric text by alignment as well as by the digits themselves. When numerals share a common height and width, columns, ticks, and repeated values line up cleanly and are faster to scan.

**Mechanism:** Lining figures keep all digits on the same height, and tabular figures keep all digits on the same width, which makes numeric text easier to compare in structured displays.

**Evidence:** The article recommends lining figures over oldstyle figures for data visualizations and recommends tabular figures over proportional figures for most visualization contexts because aligned heights and widths make tables, tooltips, and axis ticks easier to read [@muth_fonts_2022].

**Notes:** The source says proportional figures are nicer in paragraph text, but not for most chart reading tasks.

## When to use lining tabular numerals <!-- role: context -->

- **User Goal:** Let readers compare and read values exactly.
- **Task:** Look up and compare numbers across repeated labels or cells.
- **Data:** Quantitative values appear as text.
- **Chart Setting:** Numbers appear in tables, tooltips, axis ticks, or similar structured labels.
- **Audience:** Readers need quick numeric comparison rather than prose reading.
- **Success Criterion:** Values align cleanly and are easy to scan.

## When to break the lining tabular numeral rule <!-- role: exceptions -->

**Break it when:** The numbers appear in running paragraph text instead of structured chart text. **Why:** Proportional and oldstyle figures can look nicer in prose than tabular lining figures.

## Tradeoffs of lining tabular numerals <!-- role: costs -->

**Sacrifice:** You give up some of the smoother paragraph feel of proportional figures.
**Risk:** Using oldstyle or proportional figures in structured numeric text makes value comparison slower.
**Mitigation:** Keep paragraph text in proportional figures if you want, but keep chart values in lining tabular figures.

## Common lining tabular numeral mistake <!-- role: mistakes -->

**Mistake:** Using oldstyle or proportional numerals for table cells, tooltip values, or axis ticks. **Why it fails:** Different digit heights or widths make aligned numeric reading harder.

## How to check lining tabular numerals <!-- role: check -->

**Failure Sign:** Some digits sit above or below others, or the same number of digits produces different text widths.
**Quick Check:** Compare values such as 124.17 and 680.90 and confirm that they occupy the same width and keep all digits aligned in height.
**Stronger Test:** Review a table, tooltip, or tick list and confirm that repeated values align vertically without width drift.

## How to fix lining tabular numerals <!-- role: fix -->

- Enable lining and tabular figure settings in the chosen font if they are available.
- Replace the value font with one that includes lining tabular figures.
- Keep oldstyle or proportional figures only in paragraph text, not in structured chart values.
