---
id: organize-linked-data-by-semantic-relations
title: Organize linked data by semantic relations during information foraging
bibliography: references.bib
description: For information foraging on heterogeneous linked data, use semantic organization
  on interactive exploration views to improve insight and mitigate overwhelming undifferentiated
  access for analysts.
labels:
- purpose:refine
- basis:empirical
- data:network
- quality:insight:use
- lever:layout-structure
- operator:association
- audience:analyst
---

## Structure linked data by semantic relations <!-- role: advice -->

Organize heterogeneous linked data around semantic categories and explicit relations so users can move from overview to deeper exploration. For example, expose category abstractions together with views of entity dependencies, geographic correlations, and time-related correlations instead of presenting the linked data as an undifferentiated collection.

## Make linked sources explorable rather than overwhelming <!-- role: reason -->

Semantic structure turns many connected sources into recognizable types and relation paths, which supports guided search and lets users see how topics, entities, places, and time connect during information foraging.

**Mechanism:** Type-specific links and visible relations reduce the effort of finding relevant connections across many heterogeneous sources.

**Evidence:** The paper says that linked data provides type-specific linking that facilitates information exploration and guided search for overview and deeper understanding, and it describes semantics visualization as a human-centered interactive way to show categories, relations, geographic correlations, and time-related correlations in policy modeling [@kohlhammerVisualizationPolicyModeling2012].

## Use when exploring heterogeneous linked policy sources <!-- role: context -->

- **User Goal:** Find relevant issues, viewpoints, and connections that define or refine a policy problem.
- **Task:** Explore relations across multiple heterogeneous sources.
- **Data:** Semantically annotated or linked open data with explicit entity relationships.
- **Chart Setting:** An interactive exploration environment used for search, guided search, or decision support.
- **Audience:** Analysts preparing material for policy makers.
- **Success Criterion:** Users can trace meaningful relations and correlations across sources instead of only reading isolated records.

## Do not use when the output is already condensed <!-- role: exceptions -->

**Break it when:** The analysis has already isolated the essential issues and the remaining task is only to present a condensed summary to decision-makers. **Why:** The paper assigns rich exploratory visualization to information foraging and then describes analysts condensing the most relevant information for later decision support.

## Accept more visible structure in exchange for exploration <!-- role: costs -->

**Sacrifice:** A flat source-by-source listing.
**Risk:** Semantic relation views add more visible structure than a simple briefing needs.
**Mitigation:** Use the richer semantic organization during information foraging, then condense the findings for later presentation.

## Avoid flat presentations of linked sources <!-- role: mistakes -->

**Mistake:** Present linked heterogeneous sources without semantic grouping or relation views. **Why it fails:** Handling and access remain complex and overwhelming because users face too much data without topic-related structure.

## Verify that semantic paths are visible <!-- role: check -->

**Failure Sign:** Users can open many linked records but cannot see categories, relations, or correlations in the interface.
**Quick Check:** Inspect whether the display exposes semantic categories and at least one explicit relation or correlation view.
**Stronger Test:** Ask a reviewer to follow one topic across linked entities and then across either location or time from the visualization alone.

## Add semantic grouping and relation views <!-- role: fix -->

- Group the displayed information into semantic categories.
- Add explicit views of relations or dependencies between linked entities.
- Add geographic or time-correlation views for the same semantically linked information.
