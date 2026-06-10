---
id: sort-rows-by-the-most-important-value
title: Sort rows by the most important value, not by habit
bibliography: references.bib
description: For long storytelling tables, use task-driven row order on tables to
  improve insight and mitigate burying important rows below the first screen or page
  for readers who see the top of the list first.
labels:
- purpose:refine
- basis:heuristic
- chart:table
- quality:insight
- lever:scale-order
- density:dense
- scope:record-list
---

## Task-driven row order <!-- role: advice -->

Sort table rows by the most important value instead of defaulting to the first column alphabetically. For example, put the key row first, or sort by an invisible summary column such as population while keeping that helper column hidden.

## Why row order matters <!-- role: reason -->

Long tables reveal the top rows first, so default ordering determines what readers notice.

**Mechanism:** Sorting by the main comparison brings the most informative rows to the top, while habitual alphabetical order can bury the story in later rows or later pages.

**Evidence:** The post warns that sorting the first column alphabetically often does not bring the most interesting data to the top, recommends putting the most important value first or sorting by an invisible column, and says order matters even more when the table is long or paginated [@muth_tables_2019].

## Use when the top rows should carry the story <!-- role: context -->

- **User Goal:** See the most important rows early.
- **Task:** Storytelling with a long record list.
- **Data:** A table where one value or hidden summary can define importance.
- **Chart Setting:** Long or paginated table where many rows are not visible at first.
- **Success Criterion:** The most informative rows appear near the top by default.

## Do not use when alphabetical lookup is primary <!-- role: exceptions -->

**Break it when:** Readers mainly need alphabetical lookup by the first column. **Why:** Changing the order can make the table harder to use and, as the post notes, some custom sorting can make tables unreadable.

## Tradeoffs of non-alphabetical order <!-- role: costs -->

**Sacrifice:** You give up the familiar default order of the first column.\
**Risk:** Custom sorting can make some tables unreadable.\
**Mitigation:** If you are unsure, allow custom sorting so readers can choose another order.

## Common ordering mistake <!-- role: mistakes -->

**Mistake:** Alphabetizing the first column by default without checking whether that serves the story. **Why it fails:** The most important rows may stay hidden below the top of the table.

## Check whether the default order serves the story <!-- role: check -->

**Failure Sign:** The first rows are not the most interesting or informative ones.\
**Quick Check:** Compare the top of the alphabetical table with a version sorted by the main value.\
**Stronger Test:** Create a hidden helper column for importance and see whether sorting by it moves better rows onto the first screen or page.

## Fix the row order <!-- role: fix -->

- Sort the rows by the value that matters most to the story.
- Use a hidden helper column when the best sort key should not be displayed.
- Enable custom sorting if you are not sure one default order will suit all readers.
