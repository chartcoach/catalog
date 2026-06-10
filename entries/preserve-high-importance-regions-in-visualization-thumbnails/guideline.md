---
id: preserve-high-importance-regions-in-visualization-thumbnails
title: Preserve high-importance regions when creating visualization thumbnails
bibliography: references.bib
description: For retrieval in a record-list of data visualizations, use importance-based
  thumbnailing on single-view visualizations to improve readability and mitigate unreadable
  uniform shrinkage for viewers scanning many results.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- scope:record-list
- quality:readability
- lever:layout-structure
- reading-mode:overview
- polish:focus
---

## Thumbnail cropping and carving <!-- role: advice -->

Build the thumbnail from the most important regions instead of shrinking the full visualization uniformly. For example, preserve the title, main supporting text, and extreme data regions, and remove lower-importance rows or columns to reach the target aspect ratio.

## Why importance-based thumbnails search better <!-- role: reason -->

Tiny full-image thumbnails often make text and key data regions too small to recognize quickly. A thumbnail that keeps the regions people inspect first gives readers a faster summary when they scan a grid of results.

**Mechanism:** Preserving high-importance text and key data regions makes the thumbnail easier to identify and match to a search target.

**Evidence:** In the paper’s search task, participants found the described visualization in fewer clicks with importance-based thumbnails than with uniformly resized originals, and the retained thumbnail content typically included titles, supporting text, and data extremes [@bylinskiiLearningVisualImportance2017].

## Use when thumbnails must support search <!-- role: context -->

- **User Goal:** Help readers find the right visualization in a large collection.
- **Task:** Summarize each visualization into a small preview for scanning.
- **Data:** Dense data visualizations with important text and graphical regions.
- **Chart Setting:** Single-view visualizations displayed as small thumbnails in a grid or list.
- **Audience:** Readers scanning many candidate results.
- **Success Criterion:** Readers identify the target visualization in fewer clicks.

## Do not use this when the map slices through elements <!-- role: exceptions -->

**Break it when:** The importance map is highly non-uniform within text or graphical elements. **Why:** The paper notes that this can cut off parts of elements or text in downstream thumbnailing.

## Costs of aggressive summarization <!-- role: costs -->

**Sacrifice:** Full context and exact original layout.
**Risk:** Important text or marks can be cut at the boundary of the kept region.
**Mitigation:** Soften retained boundaries with a fade to white after carving.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Uniformly resize the full visualization into a tiny thumbnail. **Why it fails:** Key text and high-value regions become too small to support fast retrieval.

## How to test the thumbnail <!-- role: check -->

**Failure Sign:** Readers need several clicks to find the target visualization in a thumbnail grid.
**Quick Check:** Compare the importance-based thumbnail side by side with a simple resized version and inspect whether the title and key supporting text remain visible.
**Stronger Test:** Run an A/B search task and compare average clicks to the target between the two thumbnail versions.

## What to change next <!-- role: fix -->

- Remove low-importance rows or columns until the thumbnail reaches the target proportions.
- Preserve the title and main supporting text inside the retained region.
- Keep the data extremes that remain visually diagnostic at small size.
- Fade carved boundaries to white so the remaining content reads as a coherent thumbnail.
