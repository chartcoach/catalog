---
id: use-symbol-map-for-absolute-regional-totals
title: Use a symbol map for absolute regional totals
bibliography: references.bib
description: For comparison of non-temporal regional totals, prefer a symbol map over
  a choropleth on geospatial data to improve fidelity and mitigate misleading area-based
  comparison for readers interpreting raw counts.
labels:
- purpose:select
- basis:heuristic
- task:compare
- chart:map:use
- chart:choropleth:avoid
- data:geospatial
- quality:fidelity
- lever:chart-family
---

## Chart family for absolute totals <!-- role: advice -->

Replace the choropleth with a symbol map when the mapped number is an absolute count rather than a rate or other relative value. For example, map total people, total cases, or total events with symbols instead of filling each region by its raw count.

## Why raw counts need a different map <!-- role: reason -->

Filled regions make raw totals look comparable even when the values are not normalized across places.

**Mechanism:** A choropleth invites readers to compare filled areas as if the numbers were directly comparable by region. A symbol map avoids using geographic area as the main cue for absolute counts.

**Evidence:** The post says choropleth maps work best for relative data, explains that raw totals are not comparable without a denominator, and recommends a symbol map for absolute data [@muth_choroplethmaps_2018].

## Use when counts are not normalized <!-- role: context -->

- **User Goal:** Compare where total amounts are larger or smaller.
- **Task:** Compare raw regional counts.
- **Data:** Absolute totals by region, not rates or per-capita values.
- **Chart Setting:** A map is already desired for regional display.
- **Audience:** Readers interpreting regional quantities.
- **Success Criterion:** Regions are not made to look comparable when the values need normalization.

## Do not use when the value is already relative <!-- role: exceptions -->

**Break it when:** The mapped value is a rate, share, or other relative measure. **Why:** The post says choropleth maps work best for relative data because those values are more comparable across regions.

## Costs of switching away from filled regions <!-- role: costs -->

**Sacrifice:** You give up the simple filled-area overview of the whole surface.
**Risk:** A symbol map can end up mainly answering where most people live.
**Mitigation:** Check whether the story is only population concentration before committing to an absolute-value map.

## Common raw-count failure <!-- role: mistakes -->

**Mistake:** Fill regions by raw totals in a choropleth. **Why it fails:** Readers compare the colors without the denominator that would make the values comparable.

## Decide between choropleth and symbol map <!-- role: check -->

**Failure Sign:** The choropleth draft asks readers to compare raw counts across regions directly.
**Quick Check:** Put the choropleth draft next to a symbol-map draft of the same totals and ask which one avoids treating the raw counts like normalized values.
**Stronger Test:** Ask whether a reader can fairly compare two regions without any population or denominator context; if not, avoid the choropleth.

## Edit the map for absolute totals <!-- role: fix -->

- Replace region fills with symbols sized by the total.
- Rewrite the unit label so it clearly states that the values are totals.
- If the real question is about rates, compute a relative measure and return to a choropleth.
- Reconsider the map if it only shows where population is concentrated.
