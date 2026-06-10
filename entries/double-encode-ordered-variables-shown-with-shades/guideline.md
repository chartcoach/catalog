---
id: double-encode-ordered-variables-shown-with-shades
title: Double-encode any ordered variable shown with shades
bibliography: references.bib
description: For quick-reading charts that use shades for an underlying order or second
  measure, prefer color encoding on values already visible in position, order, size,
  or an obvious companion key to improve readability and mitigate hidden second-variable
  encodings for readers interpreting color.
labels:
- purpose:refine
- basis:heuristic
- quality:readability
- lever:encoding
- channel:color-lightness:use
- measure:multi
---

## Visible color meaning <!-- role: advice -->

Use shades for an underlying order only when readers can see the same ordered variable elsewhere in the chart or in a clear companion view. For example, color treemap rectangles by their rectangle size rather than by a different measure, keep line shades tied to a stable visible line order, or pair a color-coded scatter plot with another view that acts as a large color key.

## Why visible duplication matters <!-- role: reason -->

Readers struggle when dark and light are the only place a variable appears or when the same colors already have another job. Double-encoding makes the meaning of the shades discoverable without extra math.

**Mechanism:** When position, order, size, or a companion key repeats the same variable, readers can confirm what the shades mean instead of guessing at a hidden second signal.

**Evidence:** The article warns that coloring by values not already encoded elsewhere makes most charts hard to read and says to use shades only when it is easy to spot which value they are encoding, ideally through double-encoding or an obvious key [@muth_quantitative_vs_qualitative_2021].

## Use when color shows an underlying order <!-- role: context -->

- **User Goal:** Add an ordered color cue without slowing down reading.
- **Task:** Show an underlying rank or second measure.
- **Data:** A variable could be encoded by color in addition to size, position, or order.
- **Chart Setting:** The chart should be quick to read.
- **Success Criterion:** Readers can tell what darker and lighter mean without doing extra calculation.

## Do not use when color is the only clue <!-- role: exceptions -->

**Break it when:** The same ordered variable is not visible elsewhere and no clear companion key can be added. **Why:** Color becomes a hidden second job and the chart gets hard to decode.

## What this choice costs <!-- role: costs -->

**Sacrifice:** You give up using color as a completely independent hidden variable.
**Risk:** Repeating the variable with order, size, or a companion view can take more space.
**Mitigation:** If fast reading matters, keep shades tied to an ordered cue the chart already shows.

## Common encoding failure <!-- role: mistakes -->

**Mistake:** Color bars, treemap items, or grouped series by a second measure that is not otherwise shown. **Why it fails:** Readers cannot tell what the shades rank, and the existing marks already demand attention for another job.

## How to test whether the color meaning is visible <!-- role: check -->

**Failure Sign:** Reviewers can name the category or mark but not what darker versus lighter means.
**Quick Check:** Ask what variable the shades are encoding without pointing to explanatory text.
**Stronger Test:** If the answer is not visible in position, order, size, or a companion view, the color meaning is hidden.

## How to revise it <!-- role: fix -->

- Recolor the marks by the value already shown through size, order, or position.
- Reorder lines or other marks so the shade ranking stays visible across the chart.
- Add a companion view that repeats the color logic as a large key.
- Remove the secondary color encoding if you cannot make its meaning obvious.
