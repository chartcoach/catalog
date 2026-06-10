---
id: use-oriented-glyphs-instead-of-oriented-textures-for-average-direction
title: Use oriented glyphs instead of oriented textures for average-direction summaries
bibliography: references.bib
description: For overview summary tasks, prefer oriented glyphs on directional displays
  to improve fidelity and mitigate imprecise average-direction judgments for viewers
  summarizing local regions.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity:use
- lever:encoding
- channel:orientation:use
- channel:texture:avoid
- reading-mode:overview
---

## Put direction on glyph boundaries <!-- role: advice -->

Use oriented glyphs instead of oriented textures when viewers must summarize average direction. For example, show directional fields with line-like or arrow-like marks whose boundaries carry orientation rather than with direction embedded inside textured regions.

## Why glyph boundaries help directional summaries <!-- role: reason -->

Average orientation is read more precisely from the boundaries of objects than from internal texture. When the task is to summarize prevailing direction in a region, boundary-carried orientation gives the viewer a cleaner directional signal.

**Mechanism:** Boundary orientation is easier to average than texture orientation, so viewers can estimate overall direction more precisely.

**Evidence:** The review collates this paper as a source on aggregate and correlate-like pattern judgments. In its summary-task discussion, the paper states that average orientation is more precisely extracted from object boundaries than from internal textures and uses that result to recommend oriented glyphs over oriented textures for average-direction summaries [@zengReviewCollationGraphical2023; @szafirFourTypesEnsemble2016].

## Use when viewers need a prevailing direction <!-- role: context -->

- **User Goal:** Summarize the dominant direction within a region.
- **Task:** Estimate average orientation rather than inspect each item individually.
- **Chart Setting:** Directional displays where the same directional variable could be shown with glyph orientation or texture orientation.
- **Success Criterion:** More precise average-direction judgments across local regions.

## Do not use this as a blanket rule for other tasks <!-- role: exceptions -->

**Break it when:** The chart is not being used for average-direction summary. **Why:** The reported benefit is specific to summarizing mean orientation.

## Tradeoffs of glyph-based direction encoding <!-- role: costs -->

**Sacrifice:** You give up relying on internal texture alone to carry the directional message.
**Risk:** Texture orientation can still look directional but support less precise average-direction reading.
**Mitigation:** Keep the directional summary on glyph boundaries when that summary is the chart’s main job.

## Common failure with directional textures <!-- role: mistakes -->

**Mistake:** Encoding a summary-critical directional field as oriented texture and expecting equally precise average-direction judgments. **Why it fails:** The paper explicitly distinguishes boundary orientation from internal texture orientation in summary precision.

## Check whether direction is easy to summarize <!-- role: check -->

**Failure Sign:** Reviewers disagree about the prevailing direction in the same local region.
**Quick Check:** Compare a glyph-oriented version and a texture-oriented version of the same directional field.
**Stronger Test:** Ask reviewers to state the average direction in selected regions and compare agreement across the two versions.

## Fix the direction encoding <!-- role: fix -->

- Replace oriented textures with oriented glyphs when the task is to summarize average direction.
- Keep the directional signal on object boundaries rather than inside textured fills.
