---
id: prefer-temporal-transitions-when-next-step-options-are-equally-simple
title: Prefer a temporal transition when equally simple next-step options compete
bibliography: references.bib
description: For choosing the next slide in a linear narrative sequence, prefer temporal
  transitions on multi-view visualization presentations to improve readability and
  mitigate less favored measure, dimension, or granularity jumps for audiences following
  a guided presentation.
labels:
- purpose:refine
- basis:empirical
- task:compose
- time:ordered-time
- data:temporal
- structure:multi-view
- quality:readability
- lever:layout-structure
---

## Choose time as the next-step lever <!-- role: advice -->

Choose a time-step transition before an equally simple change in measure, dimension, or granularity. For example, after a chart for one time point, move to the same chart for the next or previous time point rather than switching to a different metric, a different grouping variable, or a broader or narrower aggregation when each option changes only one attribute.

## Why temporal transitions are preferred <!-- role: reason -->

When several next slides are equally easy to connect to the current view, audiences prefer time-based movement. A time step provides a more favored local link than an equally simple shift in what variable or level of detail is shown.

**Mechanism:** A temporal step preserves the visual frame while giving viewers a natural ordered change to track, which makes the next view feel like a better continuation.

**Evidence:** In cost-constant trials where alternative next slides each changed only one attribute, participants preferred temporal transitions over granularity, dimension, and measure transitions. Dimension and measure transitions were both preferred over granularity, and no preference was found between dimension and measure [@hullmanDeeperUnderstandingSequence2013].

**Notes:** The study did not distinguish audience preferences among temporal subtypes such as forward versus reverse chronology.

## Use when several cost-1 next slides are available <!-- role: context -->

- **User Goal:** Pick the most acceptable next slide from several plausible options.
- **Task:** Local sequencing in a linear narrative presentation.
- **Data:** The visualization set includes a time variable and also supports non-temporal single-change alternatives.
- **Chart Setting:** Adjacent views keep the chart syntax stable and differ by one data attribute.
- **Audience:** Viewers following a guided presentation.
- **Success Criterion:** The chosen next step feels like the better continuation of the current view.

## Do not override a lower-cost non-temporal option <!-- role: exceptions -->

**Break it when:** The temporal option requires more attribute changes than a non-temporal option. **Why:** In the study, lower transformation cost dominated transition type preference.

## Costs of preferring temporal transitions <!-- role: costs -->

**Sacrifice:** You delay a measure, dimension, or granularity comparison that might also be important.\
**Risk:** Forcing a time step can weaken the specific comparison you want the audience to make at that moment.\
**Mitigation:** Use the temporal step only when it competes with equally simple alternatives.

## Common transition-type mistake <!-- role: mistakes -->

**Mistake:** Use a granularity change as the next slide when a same-cost temporal step is available. **Why it fails:** Granularity transitions were the least preferred local transition type in the study.

## Check same-cost next-step choices <!-- role: check -->

**Failure Sign:** The chosen next slide changes detail level, measure, or grouping even though a same-cost time step exists.\
**Quick Check:** Enumerate all candidate next slides with transition cost 1 and mark each one as temporal, measure, dimension, or granularity.\
**Stronger Test:** Show viewers the current slide plus two same-cost next-slide candidates and ask which one should appear directly after the current view.

## Fix a weak same-cost next step <!-- role: fix -->

- Replace the current next slide with the same view at another time point.
- Move the measure, dimension, or granularity change later in the sequence.
- Keep measure, dimension, and granularity constant while stepping through time.
