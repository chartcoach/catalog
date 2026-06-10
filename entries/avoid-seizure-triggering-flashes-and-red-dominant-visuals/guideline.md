---
id: avoid-seizure-triggering-flashes-and-red-dominant-visuals
title: Avoid seizure-triggering flashes and red-dominant visuals
bibliography: references.bib
description: For static or active chart presentation, avoid flashing and red-dominant
  visual changes on chart content to prevent seizure risk and mitigate unsafe red
  flashes, red animation, and large red display areas for viewers with photosensitive
  seizure sensitivity.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- access:motion-safe:use
- aesthetic:color:avoid
---

## Reduce risky flashes and red motion <!-- role: advice -->

Remove flashing visual changes and red-dominant motion that can trigger seizures. For example, do not use red flashes, do not animate chart elements in red, and revise static or active views where a significant portion of the display area is red.

## Why seizure-safe visuals matter <!-- role: reason -->

Flashing content and red-dominant visual change can create a direct safety hazard for some viewers. Reducing these effects makes a chart safer to view across both its default presentation and its active states.

**Mechanism:** Removing flashes and risky red visual changes reduces the chance that the chart's presentation itself triggers a seizure.

**Evidence:** Chartability marks seizure risk as a critical perceivability failure and directs reviewers to avoid red flashes, red animation, and large red display areas that may pose risk. WCAG explains that flashing content should stay below threshold and avoid red flashes, and PEAT is provided as a review tool for detecting these hazards in rendered media [@elavskyHowAccessibleMy2022; @w3c_understanding_three; @umd_photosensitive_epilepsy].

**Notes:** Complex interactive data experiences may need more methodological attention than a check of a single rendered state.

## Use when reviewing visual safety <!-- role: context -->

- **User Goal:** Release a chart that is safe to view in every state.
- **Chart Setting:** The chart is static or active and includes flashing, animation, or large red display regions.
- **Audience:** Viewers may include people with photosensitive seizure sensitivity.
- **Success Criterion:** No default or active state presents red flashes or other seizure-risk visuals.

## Do not rely on a one-state review <!-- role: exceptions -->

**Break it when:** You use this rule as a one-state check on a complex interactive chart. **Why:** Interaction can generate additional visual sequences that also need seizure-risk review.

## Tradeoffs of removing risky motion <!-- role: costs -->

**Sacrifice:** Fast flashing emphasis and red-heavy animated attention cues are removed.\
**Risk:** Revising only the initial view can leave later interactive states risky.\
**Mitigation:** Review the full sequence of chart states and retest the rendered result.

## Common seizure-risk misses <!-- role: mistakes -->

**Mistake:** Checking only the default chart view and ignoring active states or large red display areas. **Why it fails:** Seizure risk can appear after interaction or when red occupies a significant portion of the display.

## How to test seizure risk <!-- role: check -->

**Failure Sign:** The chart flashes, animates with red, or shows red across a significant portion of the display area.\
**Quick Check:** Inspect both the default view and active states for flashing sequences and red-dominant motion.\
**Stronger Test:** Run the rendered chart media through PEAT to assess seizure risk.

## How to revise risky charts <!-- role: fix -->

- Remove flashing sequences from the chart.
- Replace red animation or red flashes with a non-flashing visual change.
- Reduce or redesign views where red occupies a significant portion of the display area.
- Recheck both default and active states after the revision.
