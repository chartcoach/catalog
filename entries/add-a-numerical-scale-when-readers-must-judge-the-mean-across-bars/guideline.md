---
id: add-a-numerical-scale-when-readers-must-judge-the-mean-across-bars
title: Add a numerical scale when readers must judge the mean across bars
bibliography: references.bib
description: For aggregate reading of grouped results, use a numerical scale on bar
  charts to improve fidelity and mitigate underestimation of the grand average for
  readers making quick mean judgments.
labels:
- purpose:refine
- basis:empirical
- scope:grouped-result
- chart:bar
- quality:fidelity
- lever:text-annotation
- component:axis:use
- reading-mode:overview
---

## Add a numerical scale for mean judgments <!-- role: advice -->

Add a numerical scale to a bar chart when readers must judge the grand average across bars. For example, use a bar chart with a visible labeled y-axis scale instead of the same chart without that scale when the task is to decide whether the average should be higher or lower.

## Why the numerical scale helps <!-- role: reason -->

A numerical scale gives readers an external reference for locating the average across bars. That reference reduces the size of the underestimation bias that appears when readers infer the mean from bar height alone, even though the bias can still remain.

**Mechanism:** The numerical scale adds a readout anchor for the bar heights, so readers do less of the average judgment from the bar shapes alone.

**Evidence:** In the collated extraction, the bar chart with a numerical scale showed less underestimation bias than comparable high-bar and low-bar versions without that scale for aggregate judgments. The original experiment also reported that mean underestimation persisted even with the numerical-scale version, so the scale mitigated rather than removed the bias [@zengReviewCollationGraphical2023; @godauPerceptionBarGraphs2016].

**Notes:** Changing bars from high to low did not materially change the underestimation pattern.

## Use when mean impression matters <!-- role: context -->

- **User Goal:** Judge the overall level or grand average across categories.
- **Task:** Decide whether the average should be higher or lower than a reference.
- **Data:** Multiple quantitative values shown across categorical groups.
- **Chart Setting:** A static bar chart that readers will scan quickly for an overall average impression.
- **Audience:** Readers making fast first-pass judgments from the chart.
- **Success Criterion:** Smaller underestimation of the grand average.

## Do not treat this as a complete fix <!-- role: exceptions -->

**Break it when:** A bias-free estimate of the grand average is required from the chart alone. **Why:** Underestimation persisted even when the numerical scale was added.

## Cost of relying on the scale alone <!-- role: costs -->

**Sacrifice:** The numerical scale reduces the bias but does not eliminate it.\
**Risk:** Treating the scale as a complete fix can leave readers with a still-biased impression of the grand average.\
**Mitigation:** Use the scale as a bias-reduction step and still verify mean judgments when exact average reading matters.

## Common failures around this fix <!-- role: mistakes -->

- **Mistake:** Trying to fix the mean-estimation problem only by making the bars taller or shorter. **Why it fails:** High-bar and low-bar versions showed the same underestimation pattern.
- **Mistake:** Assuming that adding the numerical scale makes the average judgment unbiased. **Why it fails:** The underestimation remained present in the numerical-scale condition.

## Test the chart for residual mean bias <!-- role: check -->

**Failure Sign:** Reviewers still place the perceived average below the true average.\
**Quick Check:** Show the chart with the true mean as a reference and ask whether the mean should be higher or lower; repeated "should be lower" responses indicate residual underestimation.\
**Stronger Test:** Compare the scaled bar chart against the same chart without the scale and keep the version that yields fewer underestimation responses.

## What to change next <!-- role: fix -->

- Add a visible labeled numerical y-axis scale to the bar chart.
- Re-test the chart with a quick higher-or-lower mean judgment using the true average as the reference.
- Do not treat tall-versus-short bar adjustments as a remedy for the mean-estimation problem.
- If exact unbiased mean reading is essential, do not rely on the bar chart alone.
