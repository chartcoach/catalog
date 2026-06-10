---
id: add-category-context-to-tooltip-values
title: Add category context to tooltip values
bibliography: references.bib
description: For value lookup in interactive charts and maps, use contextual tooltip
  text on hovered marks to improve readability and mitigate unlabeled number readouts
  for readers inspecting exact values.
labels:
- purpose:refine
- basis:heuristic
- quality:readability
- lever:interaction-access
- component:tooltip:use
- reading-mode:exact
---

## Contextual tooltip text <!-- role: advice -->

Write tooltips as a value plus what that value refers to, not as a naked number alone. For example, show a tooltip like a percentage plus its category or a signed change plus its measure instead of only showing the numeric value.

## Why contextual tooltips prevent lost meaning <!-- role: reason -->

Tooltips are often the place where readers inspect exact values. If the tooltip only shows a number, readers have to remember what the mark represented from somewhere else in the chart.

**Mechanism:** Repeating the category or measure inside the tooltip reminds readers what they are looking at at the exact moment they inspect the value.

**Evidence:** The source recommends that tooltips repeat what the visualization shows and gives examples such as pairing a percentage with its category and pairing a signed value with its measure instead of showing the number alone. [@muth_text_in_data_visualizations_2022]

## Use when readers inspect hovered values <!-- role: context -->

- **User Goal:** Read an exact value from a hovered mark.
- **Task:** Interpret a tooltip without relying on memory from axes, legends, or descriptions.
- **Chart Setting:** The chart or map uses hover tooltips.
- **Audience:** Readers may arrive at a tooltip after scanning other parts of the chart.
- **Success Criterion:** Each tooltip still makes sense when read on its own.

## Do not use when no tooltip interaction exists <!-- role: exceptions -->

**Break it when:** The visualization has no hover tooltip or no interactive value inspection. **Why:** The added context can only help if readers can actually access the tooltip.

## Tradeoffs of contextual tooltips <!-- role: costs -->

**Sacrifice:** You give up the shortest possible tooltip.\
**Risk:** Tooltips that contain only numbers stay brief but force readers to remember the category from elsewhere.\
**Mitigation:** Keep the added wording short and attach it directly to the value.

## Common tooltip failure <!-- role: mistakes -->

**Mistake:** Show only the numeric value in the tooltip. **Why it fails:** Readers get the exact number but not a fresh reminder of what the number means.

## Check tooltip self-sufficiency <!-- role: check -->

**Failure Sign:** A tooltip reads like a number fragment rather than a complete statement.\
**Quick Check:** Hover any mark and ask whether the tooltip still makes sense when read by itself.\
**Stronger Test:** Read several tooltips in isolation and see whether each one names the category or measure being shown.

## Fix tooltip wording <!-- role: fix -->

- Add the category or measure name directly into the tooltip text.
- Include direction or sign wording when the value is a change rather than a level.
- Rewrite tooltip strings so they read as short statements, not as detached numbers.
- Keep the exact value in the tooltip while adding the missing context words around it.
