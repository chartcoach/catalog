---
id: remove-3d-depth-cues-for-private-inspection
title: Remove 3-D depth cues for private inspection of the data
bibliography: references.bib
description: For private inspection of quantitative findings, avoid added 3-D depth
  cues on line or bar charts of 2-D data to improve readability and mitigate presentation-oriented
  embellishment for analysts using the graph themselves.
labels:
- purpose:refine
- basis:empirical
- audience:analyst
- lever:encoding
- quality:readability
- aesthetic:style:avoid
---

## Keep working views flat <!-- role: advice -->

Remove 3-D depth cues when the graph is mainly for your own understanding of the data. For example, keep a 2-D area line or 2-D area bar for private inspection instead of a 3-D volume version meant to impress or stand out.

## Why flat views fit self-use <!-- role: reason -->

A self-use graph does not need presentation flourish, so redundant depth cues are less useful there.

**Mechanism:** Flat rendering keeps the display focused on the data itself, which better matches a chart used to understand what is going on for your own purposes.

**Evidence:** In the paper's preference studies, 2-D graphs were preferred more for one's own use than for showing others, and the forced-choice test favored the 2-D area graph over the 3-D volume graph for self-use [@levyGratuitousGraphicsPutting1996].

## Use when the chart is for your own reading <!-- role: context -->

- **User Goal:** Understand what is going on in the data yourself.
- **Task:** Inspect the data privately rather than present it.
- **Data:** 2-D quantitative data already planned as a line or bar graph.
- **Chart Setting:** A static graph where 3-D depth cues are optional.
- **Audience:** The analyst or chart maker.
- **Success Criterion:** The graph feels better suited to your own inspection than a more presentation-oriented alternative.

## Do not use when the chart is mainly for presentation or memory <!-- role: exceptions -->

- **Break it when:** The chart is being prepared mainly for other people. **Why:** The preference for 2-D was tied to self-use and weakened outside that setting.
- **Break it when:** The chart must be memorable later without referring back to it. **Why:** Under memory-focused conditions, 3-D graphs were preferred more often.

## Costs of keeping the working view flat <!-- role: costs -->

**Sacrifice:** Some presentation flair.
**Risk:** The chart may feel less striking if reused unchanged in a talk or slide.
**Mitigation:** Reevaluate the depth treatment if the audience or purpose changes from self-use to presentation.

## Common misuse of private-inspection views <!-- role: mistakes -->

**Mistake:** Adding 3-D shading to the version you use to inspect the data yourself. **Why it fails:** The added depth is a presentation-oriented flourish that was less preferred for self-use.

## Check whether the chart is really a working view <!-- role: check -->

**Failure Sign:** You are using a showier 3-D version even though the chart is staying private.
**Quick Check:** Ask whether the current version is for your own reading or for other people; if it is for yourself, compare it against a flat version.
**Stronger Test:** Choose between flat and 3-D versions by asking which one you would keep if no one else were going to see it.

## Fix the working view <!-- role: fix -->

- Remove depth shading from the chart you use for your own inspection.
- Redraw a 3-D volume line or bar as a 2-D area version for the private working copy.
- Reassess depth only if the same chart later becomes presentation material.
