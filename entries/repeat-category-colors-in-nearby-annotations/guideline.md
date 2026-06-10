---
id: repeat-category-colors-in-nearby-annotations
title: Repeat category colors in nearby annotations
bibliography: references.bib
description: For annotated color-encoded visualizations, use category-colored annotation
  text on statements tied to specific nearby data points to improve readability and
  mitigate eye-travel back to the color key for readers interpreting highlighted categories.
labels:
- purpose:refine
- basis:heuristic
- quality:readability:use
- lever:text-annotation
- component:annotation:use
- polish:annotation
- aesthetic:color:use
---

## Category-colored annotations <!-- role: advice -->

Reuse category colors in annotations placed right next to the relevant data point. For example, color only the category term inside the annotation, not the trend word or claim, and place the annotation beside the highlighted bar, line, or point.

## Why colored annotations work <!-- role: reason -->

Annotations often sit closer to the data than the legend does. Repeating the category color in that nearby text lets readers connect the statement to the right series or group without a separate legend lookup.

**Mechanism:** A nearby color cue shortens the path between statement and data and reinforces the intended category at the moment the reader sees the annotated point.

**Evidence:** The article recommends making a statement about a specific data point, placing the annotation next to it, and coloring only the category word or phrase with the category color rather than coloring words that describe the change itself [@muth_remind_colors_2023].

## When to use category-colored annotations <!-- role: context -->

- **User Goal:** Explain or emphasize a specific data point or category.
- **Data:** Categories are already encoded with distinct colors.
- **Chart Setting:** The visualization uses annotations and a separate color key.
- **Success Criterion:** Readers can connect the annotation to the right category without returning to the legend.

## When not to use category-colored annotations <!-- role: exceptions -->

**Break it when:** The annotation is not about a specific nearby data point. **Why:** The color cue no longer reduces the distance between the statement and the data it is meant to explain.

## Costs of category-colored annotations <!-- role: costs -->

**Sacrifice:** Annotation styling becomes less uniform because part of the text carries category color.
**Risk:** Coloring too much of the sentence can make the color seem to refer to the whole claim instead of the category.
**Mitigation:** Restrict the color to the category name or phrase.

## Common annotation-color mistake <!-- role: mistakes -->

**Mistake:** Coloring the outcome words, such as “decreased” or “increased,” instead of the category name. **Why it fails:** The color then points to the event or claim rather than to the colored series or group.

## How to test annotation color reuse <!-- role: check -->

**Failure Sign:** A colored annotation still sends readers back to the legend to work out which category it names.
**Quick Check:** Inspect each annotation and confirm that only the category term is colored.
**Stronger Test:** Check that each colored annotation sits directly next to the bar, line, or point it discusses.

## How to fix annotation color reuse <!-- role: fix -->

- Move the annotation next to the exact data point it discusses.
- Recolor only the category name or phrase in the annotation.
- Remove category color from words that describe change, direction, or emphasis.
