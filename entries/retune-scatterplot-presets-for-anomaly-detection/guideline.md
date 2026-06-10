---
id: retune-scatterplot-presets-for-anomaly-detection
title: Retune the scatterplot preset for anomaly detection
bibliography: references.bib
description: For extreme-value detection, prefer task-specific preset tuning on scatterplots
  of quantitative data to improve anomaly-finding fidelity and address reuse of presets
  built for other reading tasks in preset-reuse workflows.
labels:
- purpose:refine
- basis:empirical
- task:extreme
- chart:scatter
- data:quantitative
- shape:outlier-rich
- quality:fidelity:use
- lever:encoding
---

## Scatterplot preset for anomaly finding <!-- role: advice -->

Retune the scatterplot preset when the job is to find anomalies. For example, use a task-tuned scatterplot preset instead of reusing a preset carried over from a prior correlation-reading study; in the evaluated comparison, the task-tuned design beat that reused preset on both anomaly accuracy and anomaly time.

## Why task-specific anomaly presets work <!-- role: reason -->

A scatterplot preset tuned for one reading task can emphasize the wrong tradeoffs for another. When the task shifts to finding singular points, a preset reused from correlation reading can slow search and reduce correct detections.

**Mechanism:** Task-specific scatterplot tuning aligns the visual design with anomaly finding instead of carrying forward a preset optimized or validated for a different reading task.

**Evidence:** In the collated extraction, the optimizer-generated scatterplot ranked above the prior-study scatterplot for both anomaly-detection accuracy and time, with significant differences in both metrics [@micallefPerceptualOptimizationVisual2017; @zengReviewCollationGraphical2023].

**Notes:** This guideline is supported only for the contrast between the task-tuned design and the reused prior-study preset.

## Use when the preset is being reused across tasks <!-- role: context -->

- **User Goal:** Find anomalous points in a scatterplot.
- **Task:** Find anomalies rather than estimate correlation.
- **Data:** Quantitative point data where anomalous cases can be checked against known answers.
- **Chart Setting:** A scatterplot preset is being selected or reused across tasks.
- **Success Criterion:** Correct anomaly detection and completion time both matter.

## Do not use when package-default accuracy is the main criterion <!-- role: exceptions -->

**Break it when:** The real decision is between a task-tuned preset and a standard package preset, and anomaly accuracy matters more than speed. **Why:** In this comparison, the standard package presets outperformed the task-tuned design on anomaly-detection accuracy.

## Costs of retuning for anomaly detection <!-- role: costs -->

**Sacrifice:** You may give up some anomaly-detection accuracy relative to a standard package preset.
**Risk:** You can overgeneralize and assume any task-tuned preset beats every existing preset.
**Mitigation:** Benchmark the task-tuned preset against the package preset when accuracy is the main decision criterion.

## Common preset-reuse failure <!-- role: mistakes -->

**Mistake:** Reuse a scatterplot preset validated for correlation reading as the anomaly-detection preset. **Why it fails:** The reused preset was both slower and less accurate for anomaly finding than the task-tuned preset.

## Check the anomaly preset against the reused preset <!-- role: check -->

**Failure Sign:** Reviewers miss known anomalies or take longer than expected with the current reused preset.
**Quick Check:** Run an A/B comparison between the reused preset and a task-tuned preset on a dataset with known anomalies, and record both correct detections and completion time.
**Stronger Test:** Keep the task-tuned preset only if it improves both anomaly accuracy and anomaly time over the reused preset.

## Fix the reused preset problem <!-- role: fix -->

- Create a separate scatterplot preset for anomaly detection instead of carrying over the preset from correlation reading.
- Compare the anomaly preset directly against the reused preset on data with known anomalous points.
- If anomaly accuracy is the top priority, benchmark the anomaly preset against a standard package preset before adopting it.
