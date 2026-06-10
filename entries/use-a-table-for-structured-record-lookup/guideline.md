---
id: use-a-table-for-structured-record-lookup
title: Use a table for structured record lookup
bibliography: references.bib
description: For retrieve tasks on structured record lists, use a table instead of
  text to improve lookup speed and mitigate missed reader-relevant details for readers
  seeking the entry that applies to them.
labels:
- purpose:select
- basis:heuristic
- task:retrieve
- chart:table:use
- chart:text:avoid
- quality:readability
- lever:chart-family
- reading-mode:lookup
---

## Record lookup <!-- role: advice -->

Use a table when readers need to find the entry that applies to them. For example, move structured items such as locations, ages, income ranges, names, teams, or states out of a text block and into rows and columns.

## Why table lookup works <!-- role: reason -->

A table helps readers jump to the row they care about instead of reading a paragraph from start to finish.

**Mechanism:** Tables support lookup because readers can scan for their own record, while prose forces sequential reading and makes specific facts slower to find.

**Evidence:** The post recommends tables when readers need to look up specific information and says people will often search only for the data that applies to them, which can be faster in a table than in text [@muth_tables_2019].

## Use when readers need one record <!-- role: context -->

- **User Goal:** Find the entry that applies to the reader.
- **Task:** Lookup of a specific value or record.
- **Data:** Structured text-like records such as names, places, teams, or ranges.
- **Chart Setting:** Information is currently embedded in prose or another narrative block.
- **Success Criterion:** A reader can find their own row quickly without reading everything.

## Do not use for pattern-first reading <!-- role: exceptions -->

**Break it when:** The main goal is to show an overall pattern, outlier, biggest value, or smallest value. **Why:** The post says tables are read sequentially, while charts make overall patterns and extremes easier to notice.

## Tradeoffs of replacing text with a table <!-- role: costs -->

**Sacrifice:** You give up some narrative flow from continuous prose.\
**Risk:** Important values can hide lower in the table because readers may not read the whole thing.\
**Mitigation:** Switch to a chart when the job is overview rather than lookup.

## Common prose-to-table failure <!-- role: mistakes -->

**Mistake:** Leaving repeated structured facts inside a paragraph. **Why it fails:** Readers must scan prose instead of jumping to the row that matches them.

## Check whether lookup beats prose <!-- role: check -->

**Failure Sign:** The same kinds of facts repeat in prose and readers would likely search for just one of them.\
**Quick Check:** Compare a paragraph version with a simple table and see which one lets a reviewer find one target item faster.\
**Stronger Test:** Ask whether most readers need only the row for their own location, team, age, or range rather than the full narrative.

## Fix the lookup structure <!-- role: fix -->

- Turn repeated items into rows and shared attributes into columns.
- Put the lookup key where readers can scan for it directly.
- Replace the prose block with a table when the story asks readers to find their own entry.
