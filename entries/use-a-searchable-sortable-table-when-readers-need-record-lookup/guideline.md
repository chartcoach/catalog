---
id: use-a-searchable-sortable-table-when-readers-need-record-lookup
title: Use a searchable sortable table when readers need record lookup
bibliography: references.bib
description: For retrieve tasks on record lists without a clear overall pattern, prefer
  a searchable sortable table over repeated donut charts to improve insight and mitigate
  unfocused overview scanning for readers trying to find their own record and see
  where it stands.
labels:
- purpose:select
- basis:heuristic
- task:retrieve
- scope:record-list
- chart:table:use
- chart:pie-donut:avoid
- quality:insight
- lever:chart-family
---

## Switch from overview donuts to a lookup table <!-- role: advice -->

Use a searchable sortable table when many records do not add up to one clear big-picture story and readers need to find one record that matters to them. For example, place one record per row, add search, and allow sorting by any column instead of asking readers to absorb a wall of similar donut charts.

## Why a table works better for self-lookup <!-- role: reason -->

When the data do not yield one strong pattern, a table lets readers stop chasing an overview and focus on the row that describes their own situation.

**Mechanism:** Search and sorting turn the display into a lookup tool, while the row-and-column layout lets readers scan horizontally for one record and vertically to see how it stands against others.

**Evidence:** The post argues that when the data do not add up to anything in particular, readers should be helped to focus on the strand that describes their own life, and it implements that by switching to a table with search and sortable columns so readers can find their own record and see where it stands [@mintzer_donuts_into_bars_2025].

## Use when the audience needs to find themselves in the data <!-- role: context -->

- **User Goal:** Find one personally relevant record and compare its standing with others.
- **Task:** Locate, rank, and inspect records in a long list.
- **Data:** Many records with no clear overall pattern or trend to carry a single story.
- **Chart Setting:** The current design uses many small repeated charts; the revision can support search and column sorting.
- **Audience:** Readers looking for the record that describes their own situation.
- **Success Criterion:** A reader can quickly find the relevant row and see where it stands compared with the rest.

## Do not use when one strong story already exists <!-- role: exceptions -->

**Break it when:** The records already show a clear pattern or trend that can be told as a single understandable story. **Why:** The table is proposed here specifically as an alternative when no such big-picture story is available.

## What you trade away <!-- role: costs -->

**Sacrifice:** You give up some of the immediate visual novelty of a field of mini charts.
**Risk:** The table can feel less interesting if it loses the original focal angle.
**Mitigation:** Set the default sort to the focal measure so the table keeps the original emphasis while still allowing resorting.

## Common failure around this change <!-- role: mistakes -->

**Mistake:** Keep the many mini charts and hope readers will build their own overall picture. **Why it fails:** When there is no clear overall pattern, readers cannot be expected to take everything in at once.

## How to test the choice <!-- role: check -->

**Failure Sign:** Reviewers cannot quickly find one record of interest or say where it stands.
**Quick Check:** Compare the chart and table versions by asking someone to locate a specific record and identify its standing on the focal measure.
**Stronger Test:** If search plus sortable columns let reviewers find that record and compare it faster than the chart grid, choose the table.

## What to change <!-- role: fix -->

- Put each record on its own row in a table.
- Add a search field so readers can jump to a specific record.
- Allow sorting by any column so readers can change the ranking.
- Keep the default sort on the focal measure to preserve the original angle.
