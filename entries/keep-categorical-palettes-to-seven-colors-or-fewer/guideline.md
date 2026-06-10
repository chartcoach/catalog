---
id: keep-categorical-palettes-to-seven-colors-or-fewer
title: Keep categorical palettes to seven colors or fewer
bibliography: references.bib
description: For category comparison, avoid large color sets on charts that rely on
  categorical color encoding to improve readability and mitigate repeated legend checking
  for readers.
labels:
- purpose:refine
- basis:heuristic
- data:categorical
- quality:readability
- lever:encoding
- group-cardinality:many
- polish:palette
- aesthetic:color:avoid
---

## Categorical palette size <!-- role: advice -->

Reduce the number of distinct category colors to seven or fewer when color is the main category code. For example, group categories together or move to a chart form that depends less on many category hues when your chart needs more than seven colors.

## Why fewer category colors read faster <!-- role: reason -->

Too many category colors make readers spend more effort matching hues to labels instead of reading the data pattern.

**Mechanism:** Fewer distinct hues lower the memory load of category matching and reduce back-and-forth checking of the color key.

**Evidence:** The post says that once more than seven colors represent data in a chart, quick reading becomes harder and readers need to consult the color key more often, so grouping categories or using another chart type is recommended [@muth_colors_2018].

## When to use this limit <!-- role: context -->

- **User Goal:** Compare categories quickly.
- **Data:** Many categories are distinguished primarily by color.
- **Chart Setting:** The chart relies on a legend or key to decode category hues.
- **Success Criterion:** Readers can identify categories without repeated legend lookup.

## When this limit does not apply <!-- role: exceptions -->

**Break it when:** Color is not the main way categories are distinguished. **Why:** The seven-color limit is specifically about charts where readers must tell categories apart by hue.

## Tradeoffs of fewer category colors <!-- role: costs -->

**Sacrifice:** You may need to combine smaller categories or simplify the grouping.
**Risk:** Over-grouping can hide distinctions that matter.
**Mitigation:** If grouping loses too much detail, switch to a chart form that does not depend on many category colors.

## Common palette-size mistake <!-- role: mistakes -->

**Mistake:** Adding a new hue for every additional category. **Why it fails:** The chart becomes slower to read and more dependent on the color key.

## How to check palette size <!-- role: check -->

**Failure Sign:** The chart uses more than seven data-carrying category colors.
**Quick Check:** Count the distinct category hues in the plotted data, not just the legend.
**Stronger Test:** Ask whether a reader would need to keep returning to the key to identify categories.

## How to fix palette size problems <!-- role: fix -->

- Group lower-priority categories together.
- Remove category colors that do not support the main comparison.
- Change to a chart form that relies less on many category hues.
