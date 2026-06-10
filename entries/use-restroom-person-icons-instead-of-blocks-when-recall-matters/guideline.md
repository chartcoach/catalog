---
id: use-restroom-person-icons-instead-of-blocks-when-recall-matters
title: Use gender-matched restroom person icons instead of rectangular blocks when
  recall matters
bibliography: references.bib
description: For communicating a single future risk estimate, use gender-matched restroom
  person icons on icon arrays rather than rectangular blocks to improve recall accuracy
  and mitigate overestimation for readers with lower numeracy or graphical literacy.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- scope:single-result
- quality:readability
- lever:encoding
- channel:shape:use
- knowledge:low
---

## Icon shape for recall <!-- role: advice -->

Use gender-matched restroom person icons instead of rectangular block icons in icon arrays when accurate later recall of a displayed percentage matters. For example, replace a 10×10 block grid with the same 10×10 array of male or female restroom icons, keeping the same event and non-event counts and colors.

## Why restroom person icons improve recall <!-- role: reason -->

Person-like icons changed how well readers remembered the shown percentage after the survey. The recall advantage was strongest against the most abstract option, and it mainly reduced overestimation rather than underestimation.

**Mechanism:** Restroom person icons appear to make the marked event icons easier to identify and count, which supports later memory for the displayed percentage.

**Evidence:** Accurate recall varied significantly by icon type. Restroom person icons produced higher recall than rectangular blocks overall, and the paper reports this pattern most clearly for more anthropomorphic icons versus more abstract ones, with especially notable gains among lower-numeracy and lower-graphical-literacy readers [@zikmund-fisherBlocksOvalsPeople2014].

**Notes:** The paper also found similar overall recall rates for photographs and somewhat higher recall for head outlines, but restroom person icons were the most consistent practical choice discussed by the authors.

## When to use this icon change <!-- role: context -->

- **User Goal:** Help readers remember the displayed percentage after leaving the chart.
- **Task:** Show one stated probability and support later recall of that exact value.
- **Data:** A single risk estimate shown as event versus non-event counts in an icon array.
- **Chart Setting:** A static icon array where the denominator and color coding stay fixed and only the icon type changes.
- **Audience:** Readers with lower numeracy or lower graphical literacy, though the overall recall benefit was not limited to them.
- **Success Criterion:** More readers recall the displayed value accurately, using an error tolerance of about ±2 percentage points, and fewer readers overestimate it.

## When not to rely on this icon change <!-- role: exceptions -->

**Break it when:** Your main success criterion is calibrated subjective risk judgment among lower-numeracy or lower-graphical-literacy readers rather than later recall. **Why:** In those lower-skill groups, restroom person icons improved recall but did not show an overall advantage for aligning perceived risk with displayed risk.

## Tradeoffs of restroom person icons for recall <!-- role: costs -->

**Sacrifice:** You give up the more continuous filled-area look of rectangular blocks.
**Risk:** If readers rely on overall part-whole area rather than counting, the icon swap may not improve how well their felt risk matches the displayed risk.
**Mitigation:** Use this change when memory for the shown percentage is the main outcome, not when gist-based risk calibration is the only goal.

## Common icon-shape mistake for recall <!-- role: mistakes -->

**Mistake:** Replacing blocks with other abstract icons such as ovals or smile/frown faces and expecting the same recall gain. **Why it fails:** Those icon types did not match restroom person icons on recall accuracy.

## How to check recall performance <!-- role: check -->

**Failure Sign:** Many readers remember a value that is several percentage points too high after viewing the chart.
**Quick Check:** A/B test the same icon array with restroom person icons versus rectangular blocks and compare delayed recall accuracy using a ±2 percentage point threshold.
**Stronger Test:** Split the results by numeracy or graphical literacy and verify that the recall gain is largest in the lower-skill segment.

## How to fix a weak-recall icon array <!-- role: fix -->

- Replace rectangular blocks with gender-matched restroom person icons while keeping the denominator, event count, and event/non-event color mapping unchanged.
- Re-test recall after a delay instead of judging the change only from immediate reactions.
- If your audience is mostly lower-skill and your goal is calibrated felt risk rather than memory, do not treat this icon swap as sufficient on its own.
