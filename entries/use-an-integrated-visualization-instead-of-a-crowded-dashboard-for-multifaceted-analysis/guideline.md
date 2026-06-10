---
id: use-an-integrated-visualization-instead-of-a-crowded-dashboard-for-multifaceted-analysis
title: Use an integrated visualization instead of a crowded dashboard for multifaceted
  analysis
bibliography: references.bib
description: For complex analytical tasks on multifaceted data, prefer an integrated
  single-space structure over a dashboard of separate simple views to improve insight
  and mitigate mental recombination across panels for analysts exploring multiple
  facets simultaneously.
labels:
- purpose:select
- basis:empirical
- structure:single-view:use
- structure:dashboard:avoid
- density:dense
- measure:multi
- quality:insight:use
- lever:layout-structure
---

## Choose the overall layout structure <!-- role: advice -->

Choose an integrated single-space visualization when users must inspect many related facets at once, and avoid a crowded dashboard of separate simple charts for that task. For example, combine multiple layers or aspects within one coordinated visual space instead of adding more tabular dashboard panels that viewers must mentally merge.

## Reduce mental recombination across facets <!-- role: reason -->

When related facets appear in one coordinated space, viewers can inspect relationships directly. When the same facets are split across many separate panels, viewers must mentally combine representations, and that cost rises as the dashboard grows.

**Mechanism:** Integrated structure externalizes the relationships among facets, while a crowded dashboard pushes that integration work into the viewer's head.

**Evidence:** The paper argues that simple chart-like views are ineffective for complex big-data tasks that require simultaneous exploration of many facets, and it states that crowded dashboards force users to mentally combine multiple representations while often organizing them in a generic tabular way regardless of the data relationships [@olaSimpleChartsDesign2016].

## Use when users must inspect several related facets together <!-- role: context -->

- **User Goal:** Explore multiple related aspects of the same dataset in one analysis session.
- **Task:** Perform inter-related, non-routine sensemaking tasks that depend on seeing several facets simultaneously.
- **Data:** The dataset has many attributes, relationships, levels, or layers.
- **Chart Setting:** A dashboard is becoming crowded with separate simple charts.
- **Success Criterion:** The viewer can inspect relationships across facets without mentally stitching together many isolated panels.

## Do not use when a simple task needs only one or two facets <!-- role: exceptions -->

**Break it when:** The task is simple and only one or two facets of the data matter. **Why:** The paper states that simple charts are beneficial for simple perceptual and cognitive tasks and become inadequate mainly when multifaceted analysis is required.

## Trade off modular simplicity against integrated analysis <!-- role: costs -->

**Sacrifice:** You give up some of the modular simplicity of separate small panels.
**Risk:** If the integrated view is not designed systematically, it can become labor-intensive to build and may still fail to support the task.
**Mitigation:** Structure the integrated view around the actual relationships in the data rather than around a generic panel grid.

## Avoid adding more isolated panels to solve a multifaceted task <!-- role: mistakes -->

**Mistake:** Expanding a dashboard with more separate simple charts when the analysis depends on cross-facet reasoning. **Why it fails:** The viewer must mentally combine the panels, and a generic grid layout may not match the data relationships that matter.

## Test whether the layout externalizes the relationship <!-- role: check -->

**Failure Sign:** A reviewer must look back and forth across several panels to answer one relationship question.
**Quick Check:** Compare the current dashboard with an integrated alternative and ask which one shows the needed cross-facet relationship directly.
**Stronger Test:** Inspect the arrangement of views; if the layout is mainly a tabular grid and not a reflection of data relationships, the dashboard is working against the task.

## Merge the related facets into one coordinated space <!-- role: fix -->

- Merge related facets into one integrated visual space instead of adding another isolated panel.
- Remove panels that only repeat context the integrated view can encode directly.
- Re-arrange any remaining views so their placement follows the relationships in the data rather than a generic grid.
