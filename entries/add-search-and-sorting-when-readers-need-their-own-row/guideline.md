---
id: add-search-and-sorting-when-readers-need-their-own-row
title: Add search and sorting when readers need their own row
bibliography: references.bib
description: For retrieve tasks on record-list tables with reader-specific relevance,
  use search and sortable columns on tables to improve findability and mitigate slow
  manual scanning for readers seeking their own record first.
labels:
- purpose:refine
- basis:heuristic
- chart:table
- task:retrieve
- quality:readability
- lever:interaction-access
- reading-mode:lookup
---

## Search and sortable columns <!-- role: advice -->

Add search and column sorting when different readers care about different rows. For example, include a search field for names, places, companies, or products, and let readers sort columns so they can choose the order that best fits their question.

## Why search and sorting help <!-- role: reason -->

When readers arrive with different targets, they need a fast way to reach their own row first.

**Mechanism:** Search jumps readers directly to the relevant record, and sortable columns let them reorganize the table around the field that matters most to them.

**Evidence:** The post recommends searchable and sortable tables when some information is more relevant to some readers than others, gives examples such as companies, locations, and products, and notes that a search field can solve this while taking only a bit of space [@muth_tables_2019].

## Use when relevance differs by reader <!-- role: context -->

- **User Goal:** Find the row that matches the reader's own situation.
- **Task:** Lookup within a longer record list.
- **Data:** Rows identify entities such as companies, locations, or products.
- **Chart Setting:** The same table serves readers with different priorities.
- **Success Criterion:** Readers can quickly find or reorder the row they care about.

## Do not use when everyone needs the same rows <!-- role: exceptions -->

**Break it when:** The same small set of rows matters to nearly all readers. **Why:** The rule is for tables where readers first want to find their own data.

## Tradeoffs of adding controls <!-- role: costs -->

**Sacrifice:** Search and sorting controls take some interface space.\
**Risk:** Custom sorting can make some tables unreadable.\
**Mitigation:** If space is tight, add a search field first because it uses only a little space.

## Common lookup-control mistake <!-- role: mistakes -->

**Mistake:** Forcing readers to scan the whole table for their own record. **Why it fails:** Readers who only want one row must do unnecessary manual search.

## Check whether readers need lookup controls <!-- role: check -->

**Failure Sign:** A likely first question is “Where is my company, location, or product?”\
**Quick Check:** Try finding one target row quickly without a search field or sortable columns.\
**Stronger Test:** Compare the table with and without search or sorting and see whether the target row becomes immediately reachable.

## Fix the lookup interaction <!-- role: fix -->

- Add a search field when readers are likely to look for their own row first.
- Enable column sorting so readers can reorder the table by the field that matters to them.
- Use search alone as a low-space fallback when you do not want more controls.
