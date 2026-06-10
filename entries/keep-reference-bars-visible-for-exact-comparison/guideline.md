---
id: keep-reference-bars-visible-for-exact-comparison
title: Keep the reference bar visible during exact comparison
bibliography: references.bib
description: For exact comparison of bar values across separated views, use simultaneous
  visible references on bar charts to improve comparison fidelity and mitigate memory-driven
  position misestimation for viewers making precise readings.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:bar
- structure:multi-view
- quality:fidelity
- lever:interaction-access
- reading-mode:exact
---

## Visible reference bar <!-- role: advice -->

Keep the reference bar visible when readers need an exact bar-value comparison. For example, during a bar-height adjustment or cross-view comparison, show the original bar concurrently—such as a centrally overlaid translucent reference—instead of hiding it and forcing recall.

## Why visible references work <!-- role: reason -->

The main wide-versus-tall bias arose when readers had to remember the bar after it disappeared. When the original bar remained onscreen during tracing, the aspect-ratio bias pattern largely vanished.

**Mechanism:** Simultaneous perception removes the memory step that pulls wide bars upward and tall bars downward. A visible reference lets readers match position directly instead of reconstructing it from memory.

**Evidence:** In the experiment that compared memory-based reproduction with direct tracing, the original wide-overestimate and tall-underestimate pattern appeared in memory but not when a concurrently visible reference bar stayed on screen during the response [@cejaTruthSquareAspect2021].

**Notes:** Direct tracing still showed a small general overestimation, which the paper attributes to motor overshoot rather than the aspect-ratio memory bias.

## When to keep a visible reference <!-- role: context -->

- **User Goal:** Make an exact comparison or reproduce a bar's value.
- **Task:** Compare a current bar to one from a previous display or previous step.
- **Data:** Quantitative values encoded by bar-top position.
- **Chart Setting:** The current workflow hides the earlier bar before the next judgment, and the design can keep a reference onscreen.
- **Audience:** Viewers making precision judgments rather than rough impressions.
- **Success Criterion:** Reduce memory-driven overestimation of wide bars and underestimation of tall bars.

## When this is not the right move <!-- role: exceptions -->

**Break it when:** The task is a deliberate memory test or the earlier value cannot remain onscreen during the judgment. **Why:** This rule works by removing the memory step that caused the tested bias.

## Tradeoffs of visible references <!-- role: costs -->

**Sacrifice:** This change reduces the role of recall, so it does not test what viewers remember without support.\
**Risk:** Direct tracing can still produce a small positive overshoot from motor response.\
**Mitigation:** Treat a small uniform overshoot differently from the wide-versus-tall bias pattern.

## Common visible-reference mistakes <!-- role: mistakes -->

**Mistake:** Keeping a reference available but placing it away from the response bar so the viewer must shift attention. **Why it fails:** The paper specifically used centrally co-located bars to avoid the memory transfer that eye movements or attention shifts would reintroduce.

## How to check whether memory is still driving the comparison <!-- role: check -->

**Failure Sign:** The earlier bar disappears before the exact judgment is made.\
**Quick Check:** Step through the comparison workflow; if the reader must answer after the reference vanishes, memory bias can enter.\
**Stronger Test:** Compare a sequential version with a concurrent-reference version; the wide-versus-tall signed-error pattern should shrink when the reference stays visible.

## How to keep the comparison direct <!-- role: fix -->

- Leave the earlier bar onscreen during the exact comparison.
- Overlay the reference bar directly with the adjustable or compared bar instead of separating them.
- Avoid interactions that remove the compared bar before the reader responds.
- Keep the reference and response bars centrally aligned when possible so the comparison stays perceptual rather than memory-based.
