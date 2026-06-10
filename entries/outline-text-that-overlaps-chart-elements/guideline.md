---
id: outline-text-that-overlaps-chart-elements
title: Outline text that overlaps chart elements
bibliography: references.bib
description: For labels and annotations placed over chart elements, use a text outline
  on overlapping text to improve readability and mitigate low-contrast letter edges
  for readers viewing text on marks or gridlines.
labels:
- purpose:refine
- basis:heuristic
- quality:readability
- lever:text-annotation
- channel:text:use
- polish:focus
---

## Text outlines on overlap <!-- role: advice -->

Add a text outline when labels or annotations sit on top of other chart elements. For example, place a stroke in the chart background color around letters that cross lines, filled shapes, map features, or even subtle gridlines.

## Why outlines help overlapping text <!-- role: reason -->

Text becomes harder to read when chart detail runs through the letterforms. A thin outline separates the text from the background without moving the label away from the thing it names.

**Mechanism:** The outline restores a clean edge around each letter, so the text stays legible even when marks or gridlines pass underneath it.

**Evidence:** The source recommends using a text outline whenever text sits on other elements, including subtle gridlines, and defines the outline as a stroke around the letters, often in the chart background color. [@muth_text_in_data_visualizations_2022]

## Use when text sits on marks or gridlines <!-- role: context -->

- **User Goal:** Read a label or annotation placed directly on the chart.
- **Task:** Keep on-chart text legible without moving it away from the mark it describes.
- **Chart Setting:** The text overlaps marks, map areas, or gridlines.
- **Audience:** Readers view the text in the same visual field as the data marks.
- **Success Criterion:** The text remains easy to read against the busy background.

## Do not use when text sits on a clear background <!-- role: exceptions -->

**Break it when:** The text already sits on empty, unobstructed background. **Why:** The outline is meant to solve overlap with chart elements, not plain background text.

## Tradeoffs of outlining text <!-- role: costs -->

**Sacrifice:** You add an extra stroke around the text.\
**Risk:** An outline can become unnecessary visual treatment if nothing sits behind the text.\
**Mitigation:** Reserve outlines for text that actually overlaps marks or gridlines.

## Common outline failure <!-- role: mistakes -->

**Mistake:** Place text directly over a line, fill, or gridline without an outline. **Why it fails:** The background detail cuts into the letters and makes the text harder to read.

## Check overlap legibility <!-- role: check -->

**Failure Sign:** Parts of letters visually merge with the marks or gridlines behind them.\
**Quick Check:** Inspect every label that crosses a mark or gridline and see whether its edges stay clean.\
**Stronger Test:** Compare the same text with and without the outline on the busiest background in the chart.

## Fix text-background separation <!-- role: fix -->

- Add a stroke around overlapping text.
- Match the stroke color to the chart background.
- Apply the outline to annotations, map labels, or other on-mark text that crosses visual elements.
- Remove the outline from text that already sits on plain background.
