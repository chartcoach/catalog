---
id: manually-refine-semantic-color-assignments-for-concrete-categories
title: Manually refine semantic color assignments for concrete categories
bibliography: references.bib
description: For category comparison tasks, prefer manual refinement of semantically-resonant
  hue assignments on bar charts with concrete categorical values to improve readability
  and address weaker automatic matches for categories with strong natural colors for
  readers doing quick chart readouts.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:bar
- quality:readability
- lever:encoding
- communication:workflow
- channel:color-hue:use
---

## Manual semantic color refinement <!-- role: advice -->

Review and hand-tune automatic semantic color assignments for concrete categories when those categories have strong natural colors. For example, adjust natural object categories to their representative hues and choose among multiple plausible hues based on which assignment keeps the whole set more distinct.

## Why manual refinement helps concrete categories <!-- role: reason -->

Concrete categories often have stronger and more specific color expectations than abstract ones. A manual pass can resolve ambiguous cases, pick better representative hues, and preserve distinctiveness across the full set of categories.

**Mechanism:** Manual refinement lets a designer use broader knowledge about representative colors and about conflicts inside the full category set, which can improve category identification beyond an automatic first pass.

**Evidence:** In the bar-chart experiment, expert-chosen semantically resonant assignments did not outperform algorithmic assignment overall, but they did significantly outperform algorithmic assignment for concrete categories [@linSelectingSemanticallyResonantColors2013].

**Notes:** The paper describes expert refinement as choosing representative hues, then adjusting them by hand for saliency and distinctiveness across the set.

## Use when concrete values have obvious colors <!-- role: context -->

- **User Goal:** Get the fastest possible category lookup and comparison.
- **Task:** Compare values for concrete categories whose colors are part of their appearance.
- **Data:** Categories with strong physical color associations or multiple valid representative hues.
- **Chart Setting:** A bar chart already uses a semantic color assignment, including an automatic or first-pass mapping.
- **Audience:** Readers who recognize the natural appearance of the categories.
- **Success Criterion:** A hand-refined mapping reads faster than the automatic mapping.

## Do not use when the categories are iconic or weakly colorable <!-- role: exceptions -->

**Break it when:** The categories are mainly iconic, arbitrary, or weakly associated with colors. **Why:** The paper found no overall expert advantage across all categories, so the extra manual work is most justified for concrete categories.

## Tradeoffs of manual refinement <!-- role: costs -->

**Sacrifice:** You spend more design time than with an automatic assignment alone.
**Risk:** Picking each color in isolation can make the set less distinctive even if each single color feels representative.
**Mitigation:** Choose each refined hue relative to the other categories in the set.

## Common automation failure <!-- role: mistakes -->

**Mistake:** Accept the first automatic semantic mapping unchanged for concrete categories with obvious natural colors. **Why it fails:** It can miss the extra speed benefit that expert refinement achieved on concrete sets.

## Check the concrete-category mapping <!-- role: check -->

**Failure Sign:** A concrete category is shown in a hue that conflicts with its usual appearance, or several similar categories end up too close in color.
**Quick Check:** Inspect whether each concrete item got its representative hue and whether an alternate valid hue would free a more distinctive color for neighboring categories.
**Stronger Test:** Compare the automatic mapping with a hand-refined version on a small set of representative chart-reading tasks and keep the faster accurate version.

## Repair the automatic mapping <!-- role: fix -->

- Replace nonrepresentative automatic hues with the category's representative hue.
- When a category has multiple valid hues, choose the hue that improves distinctiveness across the full set.
- Hand-tune the final colors for saliency and separation after the semantic match is in place.
