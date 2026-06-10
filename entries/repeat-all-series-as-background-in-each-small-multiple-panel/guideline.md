---
id: repeat-all-series-as-background-in-each-small-multiple-panel
title: Repeat all series as background lines in each small-multiple panel
bibliography: references.bib
description: For limited cross-series comparison over ordered time, use repeated background
  lines in small-multiple line charts to improve insight and address missing same-date
  ranking cues for readers comparing panels.
labels:
- purpose:refine
- basis:heuristic
- task:compare
- time:ordered-time
- structure:small-multiples
- quality:insight
- lever:encoding
- operator:rank
---

## Add background comparison lines <!-- role: advice -->

Repeat all series as background lines in every small-multiple panel when readers need some cross-series comparison. For example, place the full set of lines behind each featured line so readers can see which categories rank higher or lower on the same date and why panels were sorted by start or end value.

## Why repeated background lines restore context <!-- role: reason -->

Background repeats restore some shared context that separate panels remove. Readers can see whether the featured series sits above or below the rest on the same date without leaving the panel.

**Mechanism:** Repeating all lines behind the focal line adds a reference frame inside each panel, which supports higher-versus-lower judgments and clarifies start- or end-based sorting.

**Evidence:** The post recommends repeating all lines in the background of every panel to enable some cross-series comparison and to make start-value or end-value sorting more obvious [@muth_small_multiple_line_charts_2024].

## Use when small multiples still need some comparison support <!-- role: context -->

- **User Goal:** Add some cross-series comparison without leaving the small-multiple layout.
- **Task:** Judge whether a series sits above or below others on the same date.
- **Data:** Multiple time series shown as one focal line per panel.
- **Chart Setting:** Small multiples where readers still need within-panel context about the other series.
- **Success Criterion:** Readers can compare higher/lower placement within a panel, not just line shape.

## Do not use this as a substitute for exact same-date comparison <!-- role: exceptions -->

**Break it when:** Exact point-by-point comparison across categories is central to the task. **Why:** Repeated background lines enable only some comparison; small multiples still remain weak for exact same-date reading.

## Costs of adding repeated background lines <!-- role: costs -->

**Sacrifice:** You give up some visual simplicity inside each panel.
**Risk:** Readers may expect exact same-date comparison that the small-multiple layout still does not fully support.
**Mitigation:** Use repeated background lines for ranking cues, and switch to a shared plot for exact comparisons.

## Common comparison-support mistake <!-- role: mistakes -->

**Mistake:** Add repeated background lines and expect them to fully solve exact same-date comparison. **Why it fails:** The technique gives only a bit of comparison and does not replace a shared plot.

## Check whether the background lines answer the intended comparison <!-- role: check -->

**Failure Sign:** Readers still cannot tell whether the featured series ranks above or below others on a given date.
**Quick Check:** In one panel, see whether you can compare the featured line against the repeated lines at one date without leaving the panel.
**Stronger Test:** After adding repeated background lines, check whether the start-value or end-value sorting becomes more obvious.

## Edits that add cross-series context inside each panel <!-- role: fix -->

- Copy the full set of series into every panel as background lines.
- Keep the featured series visually distinct from the repeated background lines.
- Use the repeated lines especially when panels are sorted by start value or end value.
- If exact same-date comparison becomes central, replace the small-multiple layout with one shared plot.
