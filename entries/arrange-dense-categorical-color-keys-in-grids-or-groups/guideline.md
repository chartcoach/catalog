---
id: arrange-dense-categorical-color-keys-in-grids-or-groups
title: Arrange dense categorical color keys in grids or groups
bibliography: references.bib
description: For lookup in dense categorical color keys, use a grid or grouped layout
  on legends with many or long category labels to improve readability and mitigate
  overwhelming item runs for readers scanning the visualization.
labels:
- purpose:refine
- basis:heuristic
- data:categorical
- quality:readability
- lever:layout-structure
- component:legend:use
- density:dense
- reading-mode:lookup
---

## Grid layout <!-- role: advice -->

Use a grid or grouped layout for categorical color-key items when the key has many items or long labels. For example, split the items into tidy rows and columns, and group related items instead of packing everything into as few lines as possible.

## Faster skimming through shorter runs <!-- role: reason -->

Shorter vertical or grouped runs are easier to skim than one long sequence of colored labels. Grouping also gives readers visible chunks to scan instead of a single overwhelming block.

**Mechanism:** A grid or grouped layout shortens scan paths and makes the key look tidier, so readers can find a category faster.

**Evidence:** The post says that fitting categorical key items into as few lines as possible works only for a few short items, and recommends grid layouts and grouping when there are many items or long labels because they are easier to skim and look tidier. [@muth_color_keys_2023]

## Use when the key has many items to scan <!-- role: context -->

- **User Goal:** Match a chart color to its category quickly.
- **Data:** Many color-coded categories, or labels that take many letters.
- **Chart Setting:** A separate categorical color key is present and the current item run feels crowded.
- **Audience:** Readers are skimming rather than studying the key line by line.
- **Success Criterion:** Readers can find items without rereading a long horizontal run.

## Do not use when the key is already compact <!-- role: exceptions -->

**Break it when:** The key has only a few short items that fit comfortably in a compact run. **Why:** Extra grid structure adds complexity without helping skimming.

## Space cost of added structure <!-- role: costs -->

**Sacrifice:** You give up the most space-efficient single run of items.\
**Risk:** A grid or grouping can feel unnecessary on a very small key.\
**Mitigation:** Add the extra structure only when the current run feels dense or overwhelming.

## Common overcrowding failure <!-- role: mistakes -->

**Mistake:** Fit many categorical items into as few lines as possible. **Why it fails:** The key becomes overwhelming and harder to skim.

## Quick review for scanability <!-- role: check -->

**Failure Sign:** The key reads like a long crowded run of colored labels.\
**Quick Check:** Try to find one item in the middle of the key; if your eye has to track along a long run, the layout is too dense.\
**Stronger Test:** Compare the current run against a quick grid mockup and see which version is easier to skim item by item.

## Concrete edits for dense item lists <!-- role: fix -->

- Split the key into a grid with multiple rows or columns.
- Group related items into separate visual clusters.
- Add spacing between groups so the clusters read as chunks.
