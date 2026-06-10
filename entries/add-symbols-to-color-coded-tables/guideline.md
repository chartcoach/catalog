---
id: add-symbols-to-color-coded-tables
title: Add symbols when table cells are distinguished by color
bibliography: references.bib
description: For tabular status displays, prefer symbol encoding alongside color on
  table cells to improve accessibility and mitigate color-only status decoding for
  readers with color-vision deficiency.
labels:
- purpose:refine
- basis:heuristic
- chart:table
- quality:accessibility
- lever:encoding
- channel:shape:use
- needs:color-vision-deficiency
- access:noncolor:use
---

## Double-encode table status with symbols <!-- role: advice -->

Add a symbol to each color-coded table cell when color carries status. For example, pair a positive status with a check mark, pair a negative status with a contrasting symbol, and also separate the status colors by lightness so the table can be skimmed without color alone.

## Why symbols help in tables <!-- role: reason -->

Tables are often scanned quickly row by row. A symbol gives each status a second identity that survives when the cell colors become hard to distinguish.

**Mechanism:** Symbol encoding lets readers decode status from shape before or instead of decoding it from hue.

**Evidence:** The article recommends using symbols in tables when color alone cannot carry meaning, shows good/bad status double-encoded with symbols, and notes that changing the green to a lighter tone makes the statuses easier for red- and green-blind readers to skim. [@muth_colorblindness_2020]

## Use when a table uses color for status <!-- role: context -->

- **User Goal:** Scan table rows for status quickly.
- **Task:** Lookup or comparison of positive, negative, or other categorical states in a table.
- **Data:** Tabular records with status encoded by cell color.
- **Chart Setting:** A table where colors may be fixed or hard to change.
- **Audience:** Readers who may include people with color-vision deficiency.
- **Success Criterion:** The status remains clear even when color is removed or weakened.

## When to use a different noncolor channel <!-- role: exceptions -->

**Break it when:** The display is not a table. **Why:** The article assigns different noncolor encodings to different chart types, using symbols for tables but shapes for scatterplots, patterns for maps, and dotted lines for line charts.

## Costs of adding symbols <!-- role: costs -->

**Sacrifice:** You give up some visual simplicity in each cell.
**Risk:** The table can feel busier if every state gets a symbol but the colors remain hard to distinguish.
**Mitigation:** Adjust the lightness of the status colors as well, not just the symbols.

## Common table-status failure <!-- role: mistakes -->

**Mistake:** Keeping status cells color-only and leaving the colors at similar lightness. **Why it fails:** Readers still have to rely on color, and the table remains hard to skim for colorblind users.

## How to verify table symbols <!-- role: check -->

**Failure Sign:** Removing color from the table also removes the status meaning.
**Quick Check:** View the table in grayscale and see whether the symbols alone still identify each status.
**Stronger Test:** Ask a colorblind reader to scan the table and identify statuses without being told the palette.

## What to change <!-- role: fix -->

- Add a distinct symbol to each status category in the table.
- Lighten or darken the status colors so the cells differ by lightness as well as hue.
- Remove any status meaning that depends on color alone.
