---
id: increase-mark-size-until-search-speed-levels-off
title: Increase mark size until search speed levels off
bibliography: references.bib
description: For target-search tasks in dense mark-based views, use larger mark sizes
  on point- or square-mark displays to improve search speed and mitigate slow localization
  caused by tiny marks for readers scanning for one target.
labels:
- purpose:refine
- basis:empirical
- quality:readability
- lever:encoding
- reading-mode:lookup
- density:dense
---

## Mark size <!-- role: advice -->

Increase mark size for target-search views and stop once further enlargement no longer improves search speed. For example, avoid very small points or squares in a search-focused display; in the tested grids, the strongest slowdown was at and below about 0.508° visual angle, and performance was similar across the larger tested sizes.

## Why larger marks help <!-- role: reason -->

Tiny marks take longer to differentiate and parse during search. Making marks larger improves legibility quickly at first, then the benefit flattens once the marks are large enough to spot reliably.

**Mechanism:** Larger marks reduce the effort needed to detect and localize the target, but the gain is not linear and eventually plateaus.

**Evidence:** The review collated this study as evidence that larger marks can reduce response time, and the original experiments found the slowest searches at the smallest mark sizes in both grids and scatterplots, with response times flattening after larger sizes were reached [@zengReviewCollationGraphical2023; @gramazioRelationVisualizationSize2014].

## Use when the view is dense and search-focused <!-- role: context -->

- **User Goal:** Locate a known target quickly.
- **Task:** Search for a unique colored mark.
- **Data:** Many colored points or squares are shown at once.
- **Chart Setting:** Mark size is small relative to the display and the view is dense.
- **Audience:** Readers scanning one view or many views for a target.
- **Success Criterion:** Faster target localization without extra inspection.

## Do not use when overview is the job <!-- role: exceptions -->

**Break it when:** The main task is to read global patterns rather than find a single target. **Why:** The case study reported that smaller marks could be preferable for global-pattern viewing while larger marks were better for target search.

## Costs of larger marks <!-- role: costs -->

**Sacrifice:** Screen space for showing many marks.
**Risk:** Enlarging marks past the useful range uses space without comparable speed gains.
**Mitigation:** Stop increasing size once the search-time improvement plateaus.

## Common size mistake <!-- role: mistakes -->

**Mistake:** Shrink marks to fit more items when the job is target search. **Why it fails:** The smallest tested marks were consistently the slowest to search.

## Check size with a larger-mark comparison <!-- role: check -->

**Failure Sign:** Readers hesitate most on the smallest-mark version of the view.
**Quick Check:** Enlarge the current marks and repeat the same target-search task.
**Stronger Test:** Compare the current size against a moderately larger version and stop when the time gain levels off.

## Fix the mark size <!-- role: fix -->

- Enlarge tiny points or squares before adding more marks to the view.
- Hold mark size steady once further enlargement no longer improves search speed.
- If space becomes tight, reduce or summarize marks instead of shrinking them back below the useful size range.
