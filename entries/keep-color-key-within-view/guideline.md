---
id: keep-color-key-within-view
title: Keep the color key within immediate view
bibliography: references.bib
description: For long printed or scrolling visualizations, use legend placement on
  color-encoded views to improve readability and mitigate long-distance legend lookups
  for readers repeatedly checking color meanings.
labels:
- purpose:refine
- basis:heuristic
- quality:readability:use
- lever:layout-structure
- component:legend:use
- reading-mode:lookup
---

## Legend proximity <!-- role: advice -->

Keep the color key close enough that readers can recheck it without leaving their current reading position. For example, keep the key on the same printed page, make it sticky in a tall digital visualization, or repeat it so readers never need to scroll more than about one screen height to find it again.

## Why nearby legends work <!-- role: reason -->

Readers recheck color-category mappings several times when they first read a visualization. When the key stays near the data, readers can recover the mapping without long eye travel or scrolling.

**Mechanism:** Shorter distance between data and legend reduces lookup effort and helps readers keep color meanings active while reading.

**Evidence:** The article says every print visualization should share a page with its key, digital readers should not need to scroll farther than roughly one screen height to see it, and sticky or repeated keys are shown as concrete ways to maintain that proximity [@muth_remind_colors_2023].

**Notes:** Repeating a legend may feel redundant to the designer, but the article states that readers are less annoyed by repetition than by having to hunt for the key.

## When to use nearby legends <!-- role: context -->

- **User Goal:** Help readers keep color meanings available while reading.
- **Data:** Colors are explained by a separate color key.
- **Chart Setting:** The visualization is long in print or tall in digital and the key can move out of view.
- **Success Criterion:** Readers can verify any color without turning the page or scrolling far away from the current data.

## When not to use a separate nearby legend <!-- role: exceptions -->

**Break it when:** The title, description, or direct labels already function as the color key instead of a separate legend. **Why:** There is no separate color key that needs to stay nearby.

## Costs of nearby legends <!-- role: costs -->

**Sacrifice:** Nearby, repeated, or sticky legends use page or screen space.
**Risk:** The repeated key can feel redundant.
**Mitigation:** Keep the legend brief and accept repetition when it avoids long lookups.

## Common legend-distance mistake <!-- role: mistakes -->

**Mistake:** Showing the color key only once at the start of a long visualization. **Why it fails:** Readers still need to recheck the colors later and must scroll or move their eyes too far to do it.

## How to test legend proximity <!-- role: check -->

**Failure Sign:** A reader in the middle of the visualization cannot decode a color without a long scroll or page change.
**Quick Check:** Start from the middle of the piece and see whether the color key is visible within about one screen height.
**Stronger Test:** Review the print layout or digital scroll path and confirm that every reading position keeps a key on the same page or within one screen-height lookup.

## How to fix legend distance <!-- role: fix -->

- Move the legend onto the same printed page as the visualization.
- Make the legend sticky in a tall digital visualization.
- Repeat the legend at intervals so it reappears during scrolling.
