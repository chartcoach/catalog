---
id: limit-small-multiple-panels-to-message-relevant-categories
title: Limit small-multiple panels to message-relevant categories
bibliography: references.bib
description: For story-focused trend displays with many categories, prefer selective
  panel inclusion on small-multiple line charts to improve insight and address overlong
  scanning and scrolling for readers navigating many panels.
labels:
- purpose:refine
- basis:heuristic
- structure:small-multiples
- quality:insight
- lever:layout-structure
- group-cardinality:many
- communication:framing
---

## Trim the panel set <!-- role: advice -->

Limit small-multiple panels to the categories that support the takeaway. For example, remove extra panels when readers would otherwise have to scan dozens of categories or scroll a long way on mobile, and move a complete view into a searchable table with sparklines if all categories must remain available.

## Why fewer panels sharpen the story <!-- role: reason -->

Panel count controls how much scanning work the layout asks of readers. Fewer panels focus attention on the intended takeaway instead of turning the chart into an unguided search.

**Mechanism:** Reducing panels shortens scanning and scrolling, especially on mobile, and keeps the visible set aligned with the story the chart is trying to tell.

**Evidence:** The post advises keeping fewer panels than you initially plan, choosing the ones that support the point, checking mobile scrolling, and using sparklines in a searchable table if all categories must be shown [@muth_small_multiple_line_charts_2024].

## Use when the panel grid is doing too much <!-- role: context -->

- **User Goal:** Show the key categories in a story-driven small-multiple display.
- **Data:** Many categories, each with its own line panel.
- **Chart Setting:** A panel grid that may require long scanning or mobile scrolling.
- **Success Criterion:** Readers reach the main takeaway without hunting through dozens of panels.

## Do not use when every category must remain visible in the chart <!-- role: exceptions -->

**Break it when:** You need to show all categories rather than a selected story-supporting subset. **Why:** Removing panels hides part of the data; a searchable table with sparklines is the suggested fallback.

## Costs of trimming the panel list <!-- role: costs -->

**Sacrifice:** You give up complete in-chart coverage of every category.
**Risk:** Cutting too aggressively can stop the chart from giving a truthful picture of the situation.
**Mitigation:** Keep the panels that support the point while still preserving a truthful overall picture, or move the full set to a searchable table with sparklines.

## Common panel-count mistake <!-- role: mistakes -->

**Mistake:** Show dozens of panels and ask readers to find the interesting bits on their own. **Why it fails:** The chart becomes a long scan, especially on mobile.

## Check the panel load on a small screen <!-- role: check -->

**Failure Sign:** The chart takes a long time to scroll through or feels like a search task.
**Quick Check:** View the chart on a mobile screen; if it takes long to scroll through all panels, you still have too many.
**Stronger Test:** Remove panels until the remaining set still supports the intended takeaway and still gives a truthful picture.

## Edits that reduce panel overload <!-- role: fix -->

- Remove categories that do not support the intended takeaway.
- Check the chart on a mobile screen and reduce panels until the scroll is manageable.
- If all categories must remain available, move the complete set into a searchable table with sparklines.
