---
id: match-annotation-colors-to-data-colors
title: Color annotations to match the data they describe
bibliography: references.bib
description: For explaining map patterns that readers can explore in any order, use
  annotation colors that match the data colors on the map to improve readability and
  mitigate annotations overshadowing the data for readers scanning across the page.
labels:
- purpose:refine
- basis:heuristic
- chart:map
- quality:readability
- lever:text-annotation
- channel:color-hue:use
- polish:hierarchy
- reading-mode:overview
---

## Match annotation color to data color <!-- role: advice -->

Color annotation text and connectors with the same hues used for the data they describe. For example, reuse each category’s map color for its related annotation so the note sits back onto the map instead of jumping off it.

## Why shared colors reduce annotation dominance <!-- role: reason -->

Annotations compete with data when they use a louder color language than the map itself. Matching the data colors keeps the notes visually connected to the marks and lets readers explore the map in their own order.

**Mechanism:** Shared colors make annotations feel like part of the display, which lowers their visual priority and preserves the data as the main thing readers see.

**Evidence:** The post recommends reusing the data colors for annotations so they sit back onto the map instead of jumping off it, especially when the patterns can be explored in any order rather than being read immediately [@mintzer_map_annotations_2024].

## Use when the map can be scanned in any order <!-- role: context -->

- **User Goal:** Point out several interesting patterns without forcing a reading sequence.
- **Task:** Let readers wander across the map and discover annotations as they go.
- **Data:** A map with color-coded categories or groups.
- **Chart Setting:** Multiple annotations compete with the mapped marks for attention.
- **Audience:** Readers scanning across the page rather than reading a fixed sequence.
- **Success Criterion:** The data remains visually primary while the annotations stay available.

## Do not use when the annotation must demand immediate attention <!-- role: exceptions -->

**Break it when:** The annotation needs to be read right away instead of discovered during scanning. **Why:** Matching the data colors intentionally reduces the annotation’s urgency.

## What you trade away <!-- role: costs -->

**Sacrifice:** You lose some immediate annotation salience.\
**Risk:** The notes may recede too much if they also need strong emphasis.\
**Mitigation:** Use this treatment when readers can explore the patterns in any order.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Color annotations with a contrasting attention-grabbing hue unrelated to the data. **Why it fails:** The annotations jump off the map and overshadow the mapped marks.

## How to test it <!-- role: check -->

**Failure Sign:** The annotation text grabs attention before the data pattern does.\
**Quick Check:** Compare a version with shared data colors against a version with contrasting annotation colors.\
**Stronger Test:** Scan the page with no fixed reading order and check whether the annotations still feel subordinate to the data.

## What to change <!-- role: fix -->

- Apply each data category’s hue to the related annotation text.
- Apply the same hue to the annotation’s circle or connector.
- Remove annotation colors that pull more attention than the mapped data.
