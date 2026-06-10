---
id: use-distinct-hues-to-track-intertwined-lines
title: Use distinct hues when readers must track intertwined lines
bibliography: references.bib
description: For trend comparison in dense multi-line displays, use hue-based line
  colors on ordered-time charts to improve readability and address hard-to-follow
  shade ramps for readers tracking the same series across crossings or panels.
labels:
- purpose:refine
- basis:heuristic
- chart:line
- time:ordered-time
- density:dense
- quality:readability
- lever:encoding
- channel:color-hue:use
---

## Line tracking with hue <!-- role: advice -->

Use distinct hues when the main task is to follow multiple intertwined lines, even if the lines also have a rank. For example, in a faceted time-series chart with several closely packed series, keep each series in a different hue rather than a sequential ramp if readers need to follow the same line from panel to panel.

## Why hue helps with entangled lines <!-- role: reason -->

Distinct hues separate nearby lines more clearly than neighboring shades of one ramp. A shade ramp may preserve rank, but readers do not readily notice that order in a busy line chart and may lose the individual series instead.

**Mechanism:** Hue differences make each line easier to pick out across crossings and across panels, while same-hue ramps ask readers to notice subtle lightness steps at the same time.

**Evidence:** The article concludes that hues can work better than shades in entangled line charts because they make the lines easier to distinguish, even when the designer also wants to preserve a ranking across multiple panels [@muth_quantitative_vs_qualitative_2021].

## Use when series identity matters most <!-- role: context -->

- **User Goal:** Let readers follow the same series across time and across panels.
- **Task:** Track individual trends.
- **Data:** Several line series are shown together.
- **Chart Setting:** The lines are closely packed, cross, or appear in multiple panels.
- **Success Criterion:** Readers can stay on the intended line without losing it.

## Do not use when rank is the main message <!-- role: exceptions -->

**Break it when:** The lines stay in the same visible order across the chart and the priority is the ranking itself rather than series identity. **Why:** Ordered shades can then reinforce that stable rank more directly.

## What this choice costs <!-- role: costs -->

**Sacrifice:** You lose an immediate low-to-high color cue.
**Risk:** Readers may not see any ranking in the palette.
**Mitigation:** If rank still matters, reinforce it through visible line order as well.

## Common line-color failure <!-- role: mistakes -->

**Mistake:** Use a sequential ramp to encode rank on an entangled line chart. **Why it fails:** Neighboring lines are harder to tell apart, and readers may miss the intended ranking in the colors.

## How to test line tracking <!-- role: check -->

**Failure Sign:** Reviewers lose a series at line crossings or when moving between panels.
**Quick Check:** Ask someone to follow one series from the first panel to the last.
**Stronger Test:** Ask what the colors mean besides identity; if the intended ranking is not obvious, the shade cue is too subtle for this chart.

## How to revise it <!-- role: fix -->

- Recolor the lines with distinct hues.
- Keep each series in the same hue across panels.
- If rank still matters, reinforce it with visible line order.
