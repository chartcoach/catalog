---
id: reduce-mark-quantity-when-similar-marks-cannot-be-grouped
title: Reduce mark quantity when similar marks cannot be grouped
bibliography: references.bib
description: For target-search tasks in dense views, avoid high mark counts on weakly
  grouped mark displays to improve search speed and mitigate slow serial scanning
  for readers locating a single target.
labels:
- purpose:refine
- basis:empirical
- quality:readability
- lever:layout-structure
- reading-mode:lookup
- density:dense
---

## Mark quantity <!-- role: advice -->

Reduce the number of visible marks when similar marks cannot be organized into clear groups. For example, use a reduced-count or summarized point- or square-mark view instead of keeping a full randomly interleaved set in a search-focused display.

## Why fewer ungrouped marks help <!-- role: reason -->

When marks are not grouped, readers must inspect more individual items as set size grows. Search time rises with quantity in random or weakly grouped views, while grouped layouts stay much less sensitive to added marks.

**Mechanism:** Weak grouping forces serial search, so each added mark increases the amount of visual inspection needed to find the target.

**Evidence:** The review collated this study, and the original experiments showed that increasing set size slowed target search in random layouts and scatterplots, whereas set size had little effect in grouped grid displays [@zengReviewCollationGraphical2023; @gramazioRelationVisualizationSize2014].

## Use when the view is dense and ungrouped <!-- role: context -->

- **User Goal:** Locate one target quickly.
- **Task:** Search in a dense display.
- **Data:** Many discrete marks are shown at once.
- **Chart Setting:** Similar marks are randomly arranged or only weakly grouped.
- **Audience:** Readers scanning for one item rather than studying an overall pattern.
- **Success Criterion:** Lower search time as more data are added.

## Do not use when marks already pop out <!-- role: exceptions -->

**Break it when:** Similar marks are already strongly grouped by similarity. **Why:** In grouped displays, adding more marks had little effect on search time.

## Costs of reducing mark quantity <!-- role: costs -->

**Sacrifice:** Showing every mark at once.
**Risk:** Summarizing or reducing marks can limit tasks that need a fuller representation of the data.
**Mitigation:** Keep the fuller representation available when those other tasks matter.

## Common quantity mistake <!-- role: mistakes -->

**Mistake:** Keep all marks in a random layout just because they fit on the screen. **Why it fails:** Search time grows with set size when readers must inspect marks serially.

## Check density with an A/B search test <!-- role: check -->

**Failure Sign:** Search gets much slower as the same view adds more randomly arranged marks.
**Quick Check:** Compare the current view with a reduced-count or summarized version on the same target-search task.
**Stronger Test:** Time a known-target search at the current density and at a lower density.

## Fix the density <!-- role: fix -->

- Reduce the number of visible marks in the search-focused view.
- Summarize the data when showing every mark is not required for the task.
- If order is free, combine the reduced-count view with spatial grouping of similar marks.
