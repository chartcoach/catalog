---
id: remove-3d-depth-cues-for-immediate-decisions
title: Remove 3-D depth cues when the chart must support an immediate decision
bibliography: references.bib
description: For immediate decision support, avoid added 3-D depth cues on line or
  bar charts of 2-D quantitative data to improve readability and mitigate memory-oriented
  embellishment for decision-makers using the figure right now.
labels:
- purpose:refine
- basis:empirical
- audience:decision-maker
- reading-mode:exact
- lever:encoding
- quality:readability
- aesthetic:style:avoid
---

## Flatten the rendering for immediate use <!-- role: advice -->

Remove gratuitous 3-D depth cues when a chart must help people decide now. For example, use a 2-D area line or 2-D area bar instead of a 3-D volume version when the figure is meant for immediate use rather than later recall.

## Why flat rendering fits immediate use <!-- role: reason -->

Extra depth cues add visual flourish that can make a chart stand out, but that same flourish does not match a task centered on immediate use.

**Mechanism:** A flat rendering keeps attention on the values instead of on redundant depth cues, which better fits charts meant to support a decision right away.

**Evidence:** In the paper's preference studies, 2-D graphs were chosen more often than 3-D graphs when the chart was for immediate use, while 3-D graphs were preferred more when memorability was emphasized [@levyGratuitousGraphicsPutting1996].

## Use when the decision happens now <!-- role: context -->

- **User Goal:** Support a decision that must be made immediately.
- **Task:** Help viewers use the chart right now rather than remember it later.
- **Data:** 2-D quantitative data already planned as a line or bar graph.
- **Chart Setting:** A static graph where 3-D depth cues are optional.
- **Audience:** Decision-makers using the figure in the moment.
- **Success Criterion:** Viewers judge the chart as better for immediate use than a 3-D alternative.

## Do not use when later recall is the main goal <!-- role: exceptions -->

**Break it when:** The chart is being designed mainly so viewers will remember it later without referring back. **Why:** Under memory-focused conditions, 3-D graphs were preferred.

## Costs of removing depth cues <!-- role: costs -->

**Sacrifice:** Some visual punch and memorability.
**Risk:** The chart may feel less striking in a presentation setting.
**Mitigation:** Reintroduce depth only when delayed recall, not immediate use, is the main requirement.

## Common misuse of flat rendering <!-- role: mistakes -->

**Mistake:** Keeping 3-D shading because it looks more impressive even though the figure is for a same-day decision. **Why it fails:** The preference pattern linked 3-D styling to memorability, not to immediate use.

## Check whether depth is hurting the immediate-use goal <!-- role: check -->

**Failure Sign:** Reviewers say the 3-D version looks memorable or showy, but not better for deciding now.
**Quick Check:** Compare flat and 3-D versions of the same chart and ask which one is better for making the decision right away.
**Stronger Test:** Ask intended viewers to choose the version they would keep on screen while making the decision now.

## Fix the rendering choice <!-- role: fix -->

- Remove depth shading from the current line or bar chart.
- Redraw a 3-D volume line or bar as its 2-D area version.
- Keep the flat version for the decision-facing display when the same data could also be shown in a more memorable form later.
