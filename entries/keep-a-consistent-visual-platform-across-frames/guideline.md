---
id: keep-a-consistent-visual-platform-across-frames
title: Keep a consistent visual platform across consecutive frames
bibliography: references.bib
description: For step-by-step narrative reading, use a consistent visual platform
  on slideshow or tabbed views to improve readability and mitigate viewer reorientation
  for readers following transitions.
labels:
- purpose:refine
- basis:empirical
- structure:multi-view
- quality:readability:use
- lever:layout-structure
- polish:consistency
---

## Stable frame layout <!-- role: advice -->

Keep the panel layout, base map, or chart scaffold fixed across consecutive frames, and change only the content that advances the story. For example, keep the same two-panel slideshow layout while updating the text and line chart, or reuse the same map base across tabs so readers can switch topics without losing their place.

## Why a stable frame works <!-- role: reason -->

A stable frame lets readers spend attention on the changing evidence instead of repeatedly re-finding where the chart, legend, and explanatory text moved. It supports orientation during transitions and reduces the chance that narrative steps feel like disconnected scenes.

**Mechanism:** Shared layout gives readers a persistent reference frame, so updates are read as changes within one story space rather than as unrelated resets.

**Evidence:** The analyzed narratives repeatedly used a consistent visual platform to help viewers stay oriented across slide changes and tab switches, and the paper identifies this as a recurring visual-structuring tactic for narrative visualization [@segelNarrativeVisualizationTelling2010].

## Use when the narrative advances through repeated views <!-- role: context -->

- **User Goal:** Follow an authored sequence without losing place between steps.
- **Task:** Read successive updates to the same topic or scene.
- **Chart Setting:** Slide shows, tabbed graphics, or repeated views that update text, marks, or filters over time.
- **Audience:** Readers who need help staying oriented while the story moves.
- **Success Criterion:** Readers can identify what changed in each step without re-learning the whole layout.

## Do not rely on this alone when the representation changes fundamentally <!-- role: exceptions -->

**Break it when:** The story changes chart type or scene substantially. **Why:** Those changes need an explicit transition cue rather than only a stable frame.

## Costs of a stable frame <!-- role: costs -->

**Sacrifice:** You give up some freedom to redesign each step independently.\
**Risk:** If the representation changes but the frame looks almost identical, readers may miss that a deeper shift happened.\
**Mitigation:** Keep the frame stable for same-scene updates, and make major representation changes explicit.

## Common failure with stable frames <!-- role: mistakes -->

**Mistake:** Rebuilding the full layout between steps even when the narrative stays in the same scene. **Why it fails:** Readers must repeatedly hunt for the chart, legend, and text instead of focusing on the new point.

## How to check frame stability <!-- role: check -->

**Failure Sign:** Adjacent steps look like unrelated pages rather than updates to one story space.\
**Quick Check:** Step through neighboring frames and see whether the main panels, axes, or map base stay in the same positions.\
**Stronger Test:** If a chart type changes, verify that the change is explicitly signaled rather than silently swapped into the old frame.

## How to fix frame instability <!-- role: fix -->

- Keep panel positions, axes, map bases, and other major scaffolds fixed across adjacent frames.
- Update only the marks, annotations, or text that carry the next story point.
- When the representation must change, add an explicit staged transition instead of silently replacing the whole scene.
