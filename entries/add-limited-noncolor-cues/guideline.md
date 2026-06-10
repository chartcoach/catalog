---
id: add-limited-noncolor-cues
title: Add a small set of noncolor cues when color alone is not enough
bibliography: references.bib
description: For multi-category charts where color alone is insufficient, use a small
  set of noncolor indicators on marks to improve accessibility and mitigate category
  confusion for readers who may not distinguish colors well.
labels:
- purpose:refine
- basis:heuristic
- lever:encoding
- access:noncolor:use
- needs:color-vision-deficiency
- group-cardinality:many
- quality:accessibility:use
---

## Layer in one extra cue type <!-- role: advice -->

Add one extra noncolor cue when colors alone do not separate categories clearly. For example, vary symbol shape in a scatterplot or symbol map, add patterns in bars or columns, or change line width, dashes, or opacity in a line chart.

## Reduce reliance on hue alone <!-- role: reason -->

Noncolor cues give readers another way to distinguish categories when hue differences are weak or unavailable to them. They work best as a limited supplement, because too many cue types become hard to decode.

**Mechanism:** A second visual cue lets readers separate categories even when colors are similar, but each added cue increases decoding effort.

**Evidence:** The post recommends symbols, patterns, line width, dashes, and opacity as additional indicators, and it explicitly warns not to use more than three or four different ones because the chart will likely become hard to decipher; it also notes that they work well in combination with colors [@muth_fewer_colors_2022].

## Use when hue differences are not sufficient <!-- role: context -->

- **User Goal:** Make categories distinguishable without relying on color alone.
- **Task:** Separate many categories in the same chart.
- **Data:** Multiple categories are encoded on the same display.
- **Chart Setting:** The chart type supports shapes, patterns, line styles, widths, or opacity changes.
- **Audience:** Readers who may not distinguish hues reliably.
- **Success Criterion:** Categories remain distinguishable even when color alone is weak.

## Do not use when you need too many cue types <!-- role: exceptions -->

**Break it when:** The chart would require more than three or four distinct noncolor indicators. **Why:** The display will likely become hard to decipher.

## Accept some extra encoding complexity <!-- role: costs -->

**Sacrifice:** The chart gains another layer of visual coding.
**Risk:** Too many different cue types can become harder to decode than the color problem they were meant to solve.
**Mitigation:** Keep the set small and pair it with color rather than replacing color with many different cues.

## Avoid piling on many cue systems <!-- role: mistakes -->

**Mistake:** Adding many shapes, patterns, widths, and dash types at once. **Why it fails:** The chart becomes hard to decipher.

## Count the distinct cue types <!-- role: check -->

**Failure Sign:** The chart uses a growing list of different noncolor treatments to separate categories.
**Quick Check:** Count the distinct shapes, patterns, widths, dash types, or opacity treatments.
**Stronger Test:** Keep the treatment only if readers can still tell categories apart with no more than three or four noncolor cue types.

## Reduce and pair the extra cues <!-- role: fix -->

- Choose one noncolor cue type that fits the chart’s marks.
- Limit the chart to no more than three or four distinct noncolor indicators.
- Pair the noncolor cue with the existing color encoding instead of multiplying both systems.
