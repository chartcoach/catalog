---
id: use-multiplexed-numerals-when-bolding-table-values
title: Use multiplexed numerals when bolding table values
bibliography: references.bib
description: For exact reading of highlighted values in tables, use multiplexed numerals
  on bold and regular table text to improve readability and mitigate alignment shifts
  when emphasized numbers change weight for readers scanning columns.
labels:
- purpose:refine
- basis:heuristic
- chart:table
- data:quantitative
- quality:readability
- lever:text-annotation
- reading-mode:exact
- polish:hierarchy
---

## Keep bold table values the same width <!-- role: advice -->

Use a multiplexed font when table values switch between regular and bold. For example, bold a key number in a column only if the font keeps the same character widths across weights so the alignment does not move.

## Why multiplexed numerals work <!-- role: reason -->

Bold values are useful in tables, but ordinary fonts often make bold text wider than regular text. Multiplexed widths preserve the table's structure while still allowing weight-based emphasis.

**Mechanism:** When regular and bold characters keep the same width, bold emphasis does not shift column alignment or row rhythm.

**Evidence:** The article explains that multiplexed fonts keep each character and figure at the same width in each font weight and recommends them for tables because bold text in most fonts is otherwise wider than regular text, which makes highlighted numbers harder to align cleanly [@muth_fonts_2022].

## When to use multiplexed numerals <!-- role: context -->

- **User Goal:** Highlight some table values without disturbing alignment.
- **Task:** Compare values down a column while also noticing emphasis.
- **Data:** Quantitative values are shown in table cells.
- **Chart Setting:** A table uses both regular and bold text for values.
- **Audience:** Readers are scanning columns for exact values.
- **Success Criterion:** Bolded values stand out while the table stays aligned.

## When to break the multiplexed numeral rule <!-- role: exceptions -->

**Break it when:** The table uses only one font weight for its values. **Why:** Multiplexed widths matter when regular and bold text must occupy the same space.

## Tradeoffs of multiplexed numerals <!-- role: costs -->

**Sacrifice:** You limit your font choice to typefaces that keep widths constant across weights.
**Risk:** If you use an ordinary font, bold values can widen and disturb table alignment.
**Mitigation:** Reserve multiplexed fonts for tables where weight-based emphasis is part of the design.

## Common multiplexed numeral mistake <!-- role: mistakes -->

**Mistake:** Assuming tabular figures alone will keep bolded table values aligned. **Why it fails:** In most fonts, bold text is still wider than regular text even when the digits are tabular.

## How to check multiplexed numerals <!-- role: check -->

**Failure Sign:** Bold values make a column or row appear wider than the surrounding text.
**Quick Check:** Toggle a table value between regular and bold and see whether its width changes.
**Stronger Test:** Bold several values in the same column and confirm that the column edges stay stable.

## How to fix multiplexed numerals <!-- role: fix -->

- Replace the table font with a multiplexed or uni-width font that also supports tabular lining figures.
- Recheck bold highlights after the font change and confirm that the alignment stays fixed across weights.
- If the current font widens in bold, do not use it for weight-based highlighting in tables.
