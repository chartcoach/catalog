---
id: use-the-smallest-geographic-units-available
title: Use the smallest geographic units available
bibliography: references.bib
description: For overview mapping of regional patterns, use the smallest available
  geographic units on a choropleth to improve insight and mitigate hidden within-region
  variation for readers scanning spatial structure.
labels:
- purpose:refine
- basis:heuristic
- chart:choropleth
- data:geospatial
- quality:insight
- lever:layout-structure
- reading-mode:overview
---

## Geographic unit size <!-- role: advice -->

Map data at the smallest geographic unit you can support when the goal is to reveal regional pattern. For example, use counties instead of states or smaller subnational regions instead of whole countries so local clusters and contrasts stay visible.

## Why finer units reveal more pattern <!-- role: reason -->

Large units hide internal variation that smaller units can show.

**Mechanism:** Smaller geographic units give readers a more refined picture of the data and make regional pattern easier to spot. Coarser units can flatten local differences into one average fill.

**Evidence:** The post recommends using the smallest units possible because they give readers a more refined image of the data and let them spot more regional pattern [@muth_choroplethmaps_2018].

## Use when the story is spatial pattern <!-- role: context -->

- **User Goal:** Show where regional clusters or contrasts appear.
- **Task:** Scan for local pattern in mapped values.
- **Data:** Values are available at more than one geographic aggregation level.
- **Chart Setting:** A choropleth is already chosen.
- **Audience:** Readers looking for spatial structure.
- **Success Criterion:** The map reveals local variation instead of averaging it away.

## Do not use when the larger unit is the meaningful result <!-- role: exceptions -->

**Break it when:** The result itself is decided at the larger geographic unit. **Why:** The post gives winner-takes-it-all presidential election maps as a case where a state map is more informative.

## Costs of using finer units <!-- role: costs -->

**Sacrifice:** You give up the simplicity of a coarser map.
**Risk:** A finer map can distract from the actual unit that determines the outcome.
**Mitigation:** Stay with the larger unit when the larger unit is the true reporting or decision unit.

## Common aggregation failure <!-- role: mistakes -->

**Mistake:** Map only coarse units when finer regional data is available and the goal is pattern detection. **Why it fails:** Local clusters and contrasts get averaged into broader areas.

## Check whether the geography is too coarse <!-- role: check -->

**Failure Sign:** Large regions look uniform even though the topic likely varies within them.
**Quick Check:** Compare a coarse-unit draft with a finer-unit draft and see whether the finer version reveals meaningful regional pattern.
**Stronger Test:** Ask whether the mapped outcome is actually defined at the coarse unit; if not, prefer the finer geography.

## Edit the geography level <!-- role: fix -->

- Swap the map to the smaller available geographic units.
- Rejoin the values to the finer geography before recoloring the map.
- Keep the larger units only when the larger unit is itself the informative result.
- Rewrite the framing so the map claims pattern at the level it actually shows.
