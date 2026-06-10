---
id: optimize-class-to-color-assignment-in-multiclass-scatterplots
title: Optimize class-to-color assignment in multiclass scatterplots
bibliography: references.bib
description: For cluster inspection in non-temporal analysis, prefer optimized color-hue
  assignment on multiclass scatterplots to maximize class separability and mitigate
  class-counting mistakes for analysts inspecting labeled point data.
labels:
- purpose:refine
- basis:empirical
- task:cluster
- chart:scatter
- channel:color-hue:use
- lever:encoding
- group-cardinality:many
- quality:fidelity
---

## Optimize class-to-color mapping <!-- role: advice -->

Assign hues to classes by cluster separability instead of leaving the class-to-color mapping in default or arbitrary order. For example, give more different hues to spatially neighboring or overlapping clusters, and give harder-to-separate classes colors with stronger contrast against the chart background.

## Why optimized assignment works <!-- role: reason -->

Color assignment changes whether nearby classes visually merge or separate, even when the palette itself is already reasonably discriminable. Reordering the same set of hues can make clustered structures easier to distinguish and reduce miscounting when readers inspect how many classes are visible.

**Mechanism:** Assigning more distinct hues to neighboring classes increases local visual separation, while stronger background contrast helps readers recover classes that are already hard to separate because of overlap or density.

**Evidence:** The collated review records this paper as evidence about cluster perception in color-hued scatterplots, and the paper's numerical evaluation, controlled lab study, and expert study show that optimized class-to-color assignment improves perceived class separability, reduces class-counting errors, and is usually preferred over default assignments [@zengReviewCollationGraphical2023; @wangOptimizingColorAssignment2019].

**Notes:** The paper evaluates this guidance for multiclass scatterplots with color hue encoding class labels.

## Use when class separation is the goal <!-- role: context -->

- **User Goal:** Judge how clearly classes separate in a labeled scatterplot.
- **Task:** Cluster inspection, including counting how many classes are visibly distinguishable.
- **Data:** Quantitative x/y positions with nominal class labels, especially with several classes and some overlap.
- **Chart Setting:** A multiclass scatterplot that already uses color hue to encode class membership and has a fixed background.
- **Audience:** Analysts or other readers inspecting labeled point data.
- **Success Criterion:** Fewer class-counting errors and more clearly distinguishable class structures.

## Do not use as a blanket rule outside class-separation reading <!-- role: exceptions -->

- **Break it when:** The chart's main reading task is correlation, relative mean judgment, or outlier detection instead of class separation. **Why:** The paper explicitly evaluates color assignment for class separability and notes that these other tasks need further study.
- **Break it when:** Some classes must keep fixed semantic or domain colors. **Why:** Unconstrained optimization may change those mappings unless the required colors are held fixed.

## Consider the tradeoffs of optimization <!-- role: costs -->

**Sacrifice:** You give up the convenience of leaving the software's default class-to-color order unchanged.\
**Risk:** The highest-separation assignment may feel less visually balanced or less aesthetically pleasing to some readers.\
**Mitigation:** Review a small set of high-scoring alternatives or lock required class colors before optimizing the rest.

## Avoid default or palette-only thinking <!-- role: mistakes -->

- **Mistake:** Keep the software's default class-to-color order. **Why it fails:** Default ordering can place similar hues on neighboring classes and make them barely separable.
- **Mistake:** Assume a good categorical palette is enough by itself. **Why it fails:** Even well-designed palettes can produce poor class separability when the hues are assigned to classes in the wrong order.

## Test whether the current mapping hides classes <!-- role: check -->

**Failure Sign:** Readers merge neighboring clusters or miscount the number of visible classes.\
**Quick Check:** Compare the current mapping with a reordered version that uses the same palette; if the reordered version makes more classes immediately distinguishable, the current mapping is weak.\
**Stronger Test:** Ask a few readers to count the number of classes in both versions and compare mismatches; keep the assignment with fewer counting errors.

## Change the mapping before changing the chart <!-- role: fix -->

- Reassign class hues so spatially adjacent or overlapping clusters receive more different colors.
- Give low-separability classes colors with stronger contrast against the background.
- Keep the same palette and change only the class-to-color mapping before replacing the chart or palette.
- If some class colors are mandatory, lock those assignments and optimize the remaining classes around them.
