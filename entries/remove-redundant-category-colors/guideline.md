---
id: remove-redundant-category-colors
title: Remove distinct colors when position already separates categories
bibliography: references.bib
description: For multi-category comparison charts, avoid distinct color hues on marks
  that are already separated by position or gaps to improve readability and mitigate
  redundant category coding for readers seeing the chart for the first time.
labels:
- purpose:refine
- basis:heuristic
- lever:encoding
- channel:color-hue:avoid
- group-cardinality:many
- quality:readability:use
- polish:declutter
---

## Recolor redundant category hues <!-- role: advice -->

Use one mark color when another visual variable already distinguishes the categories. For example, give bars the same color when their positions and gaps already separate them, and test whether same-colored symbols or lines still read clearly.

## Remove unnecessary decoding work <!-- role: reason -->

Redundant color coding adds a decoding step without adding new information. When position or spacing already separates marks, a shared color reduces visual clutter and lets readers focus on the structure that is already doing the categorization.

**Mechanism:** Removing unnecessary hue differences reduces the number of cues readers have to interpret and makes the chart less confetti-like without changing the underlying separation.

**Evidence:** The post recommends asking what color is doing in the chart and specifically suggests recoloring bars, symbols, or lines the same when they are already distinguished by position or another visual variable, then checking whether the chart still reads easily to a new viewer [@muth_fewer_colors_2022].

## Use when category separation already exists <!-- role: context -->

- **User Goal:** Reduce an overly colorful chart without losing meaning.
- **Task:** Compare categories that are already separated visually.
- **Data:** Many categories are present.
- **Chart Setting:** Marks are already distinguished by position, spacing, or another visual variable.
- **Audience:** People who have never seen the chart before.
- **Success Criterion:** The chart remains easy to understand after recoloring.

## Do not use when color is the only category cue <!-- role: exceptions -->

**Break it when:** Color is the only thing distinguishing the categories. **Why:** Removing the colors would remove the category separation instead of simplifying it.

## Accept less color variety <!-- role: costs -->

**Sacrifice:** You give up an extra layer of category emphasis from color.
**Risk:** Some marks may feel less individually prominent after recoloring.
**Mitigation:** Recolor the chart, step back, and keep the change only if the chart still reads clearly to someone new.

## Avoid leaving redundant hue differences in place <!-- role: mistakes -->

**Mistake:** Keeping many category hues even though position or gaps already separate the marks. **Why it fails:** The extra colors do not add information, but they do add clutter.

## Test the same-color version directly <!-- role: check -->

**Failure Sign:** The chart still looks busy even though category separation is already visible from layout.
**Quick Check:** Temporarily recolor all category marks the same and step back from the chart.
**Stronger Test:** Ask whether someone who has never seen the chart can still explain it correctly.

## Make the simplification edit <!-- role: fix -->

- Recolor all categories the same when position or spacing already distinguishes them.
- Keep the positional separation or gaps visually clear.
- Reintroduce color only for the categories that still need an extra cue.
