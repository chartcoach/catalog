---
id: use-color-to-group-or-highlight-small-multiple-panels
title: Use color to group or highlight panels in small multiples
bibliography: references.bib
description: For grouped trend reading in small-multiple line charts, use color encoding
  for grouping or emphasis to improve insight and address unnecessary category-color
  keys for readers reading titled single-line panels.
labels:
- purpose:refine
- basis:heuristic
- structure:small-multiples
- quality:insight
- lever:encoding
- aesthetic:color:use
- channel:color-hue:use
---

## Repurpose color from identity to emphasis <!-- role: advice -->

Use color in small-multiple line charts to group or highlight panels, not to identify every series. For example, drop the color key, keep line identity in the panel title, and reserve distinct colors for upward versus downward trends or for the panels you want readers to notice.

## Why color becomes available for a better job <!-- role: reason -->

In small multiples, identity is already carried by panel titles and panel separation. That frees color to signal analytical grouping or emphasis.

**Mechanism:** When each panel contains one titled line, color no longer has to separate categories, so it can highlight patterns or focal panels instead.

**Evidence:** The post states that small-multiple line charts do not need different line colors or a color key for identity, and recommends using color to group similar trends or highlight selected panels [@muth_small_multiple_line_charts_2024].

## Use when every panel already names its line <!-- role: context -->

- **User Goal:** Emphasize pattern groups or focal panels.
- **Data:** One line per panel with a panel title.
- **Chart Setting:** A small-multiple line chart where line identity is already clear without a color key.
- **Success Criterion:** Color points readers to groups or highlights instead of doing identity work.

## Do not use when color is still needed just to distinguish lines <!-- role: exceptions -->

**Break it when:** A panel still contains multiple lines that are not otherwise clearly distinguished. **Why:** Color may still be needed for basic line identification.

## Costs of repurposing color <!-- role: costs -->

**Sacrifice:** You give up category-by-category color identity.
**Risk:** If line identity is not already obvious from panel titles, readers can lose track of what each hue means.
**Mitigation:** Repurpose color only after each panel clearly identifies its own line.

## Common color mistake in small multiples <!-- role: mistakes -->

**Mistake:** Assign a different color to every line just because it is a different category. **Why it fails:** Panel titles already identify the line, so the colors stop doing useful analytical work.

## Check whether color is still doing identity work <!-- role: check -->

**Failure Sign:** Every panel line has a unique hue and the chart still needs a color key.
**Quick Check:** Cover or remove the color key; if panel titles still identify every line, color can be reassigned to grouping or highlighting.
**Stronger Test:** Scan whether only grouped or highlighted panels use distinctive color while the rest stay neutral.

## Edits that turn color into emphasis <!-- role: fix -->

- Keep line identity in the panel title instead of assigning every series a unique hue.
- Use color only for groups or the few panels you want to highlight.
- Remove the category color key if color is no longer used for identity.
