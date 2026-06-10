---
id: show-category-colors-inside-tooltips
title: Show category colors inside tooltips
bibliography: references.bib
description: For interactive visualizations with tooltips, use category-colored tooltip
  content on hovered marks to improve readability and mitigate category confusion
  when the legend is unseen or covered for readers seeking exact values.
labels:
- purpose:refine
- basis:heuristic
- quality:readability:use
- lever:interaction-access
- component:tooltip:use
- reading-mode:exact
- aesthetic:color:use
---

## Tooltip color reminders <!-- role: advice -->

Repeat the category color inside the tooltip content. For example, state the category name in its color, add a colored shape or underline next to the text, or use a category-colored background for part or all of the tooltip.

## Why colored tooltips work <!-- role: reason -->

Readers often interact with a chart before they study its legend, and the tooltip may cover the legend while it is open. Repeating the category color inside the tooltip lets the popup teach or refresh the mapping while it shows exact values.

**Mechanism:** Color inside the tooltip keeps category identity available at the exact moment the reader asks for a value, even when the legend is hidden, distant, or overlapped.

**Evidence:** The article recommends using category colors in tooltips because readers may hover before reading the key, tooltips sit closer to data than a distant legend does, and the tooltip can overlap the legend and block it from view [@muth_remind_colors_2023].

## When to use colored tooltips <!-- role: context -->

- **User Goal:** Read exact values while keeping category identity clear.
- **Data:** Colors encode categories or map classes.
- **Chart Setting:** The visualization is interactive and uses tooltips or pop-ups.
- **Success Criterion:** A reader can identify the hovered category from the tooltip alone.

## When not to rely on tooltip color reminders <!-- role: exceptions -->

**Break it when:** The visualization has no tooltips or no interaction. **Why:** Readers cannot access tooltip-based reminders.

## Costs of colored tooltips <!-- role: costs -->

**Sacrifice:** Some tooltip space goes to category cues as well as numeric values.
**Risk:** A heavily styled tooltip can compete with the exact readout.
**Mitigation:** Keep the color cue small and place it next to the category name or as a partial background treatment.

## Common tooltip-color mistake <!-- role: mistakes -->

**Mistake:** Using the tooltip only for numbers and leaving out the category color. **Why it fails:** Readers who hover before reading the legend, or while the tooltip covers it, still have to guess what the hovered color means.

## How to test colored tooltips <!-- role: check -->

**Failure Sign:** A hovered tooltip shows the value but not a clear category reminder.
**Quick Check:** Hover a mark before looking at the legend and check whether the tooltip alone tells you the category.
**Stronger Test:** Open a tooltip where it overlaps the legend and confirm that the tooltip still provides the category-color mapping.

## How to fix tooltips that lose the color mapping <!-- role: fix -->

- Add the category name in its category color inside the tooltip.
- Add a colored shape or underline next to the category text in the tooltip.
- Apply a category-colored background to the relevant part of the tooltip when text color alone is not enough.
