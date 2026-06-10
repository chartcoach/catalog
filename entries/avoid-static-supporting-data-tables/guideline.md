---
id: avoid-static-supporting-data-tables
title: Avoid static supporting data tables
bibliography: references.bib
description: For low-level data access in chart views with a supporting table, avoid
  a static table on tabular data to improve accessibility and address inflexible data
  access for users who need to consume the information in different ways.
labels:
- purpose:refine
- basis:accessibility
- chart:table
- data:tabular
- quality:accessibility
- lever:interaction-access
---

## Make the table manipulable <!-- role: advice -->

Do not leave the provided data table static. For example, let readers sort columns and filter rows, ideally with search, and if that is not possible provide a downloadable CSV.

## Why a manipulable table helps <!-- role: reason -->

Static tables force one presentation of the data. Filter, sort, and download let readers reshape low-level values in the view or tool that best matches their access workflow.

**Mechanism:** Manipulable tables reduce the effort of extracting and reorganizing values, and a downloadable CSV gives users a low-level form that can be adapted in other software.

**Evidence:** Chartability states that a provided table should not remain static and should at least be downloadable, filterable, or sortable; its notes add that a downloadable CSV often satisfies many concerns because users can reshape it in other programs, while rendered filterable and sortable tables are preferred [@elavskyHowAccessibleMy2022]. Inclusive Components likewise recommends making data tables sortable or downloadable for flexibility [@inclusive-components_inclusive_components].

**Notes:** Search is the preferred filtering affordance when a rendered table supports it.

## When this applies <!-- role: context -->

- **User Goal:** Inspect, reorganize, or reuse low-level values behind a visualization.
- **Data:** Tabular values are exposed as a supporting table.
- **Chart Setting:** The table is rendered with the visualization or provided as its tabular companion.
- **Audience:** Users may rely on assistive technology or need to consume the data in a different workflow.
- **Success Criterion:** Readers can sort, filter or search, or download the table instead of reading a fixed table only.

## When to allow a fallback <!-- role: exceptions -->

**Break it when:** Rendered filter and sort controls are not feasible, but the table can be provided as a downloadable CSV. **Why:** The source treats CSV download as an acceptable minimum because it gives users a flexible low-level form they can adapt elsewhere.

## Costs of adding table controls <!-- role: costs -->

**Sacrifice:** The table stops being a fixed rendering and gains controls or an export path.\
**Risk:** A rendered table that stays fixed still forces everyone into one presentation of the data.\
**Mitigation:** Prefer rendered filter and sort controls, and use downloadable CSV when those controls cannot be supported.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Showing a rendered table with fixed rows and columns only. **Why it fails:** The table still does not let readers sort, filter, search, or export the data in the way that suits their needs.

## How to test it <!-- role: check -->

**Failure Sign:** The table has no sort control, no filter or search, and no download option.\
**Quick Check:** Try to sort a column, filter or search rows, or download the table as CSV.\
**Stronger Test:** If none of those actions is available, treat the table as static and fail it.

## What to change <!-- role: fix -->

- Add column sorting to the rendered table.
- Add row filtering to the rendered table and include search when possible.
- Provide the table as a downloadable CSV when rendered controls are unavailable.
