---
id: prefer-tables-over-stacked-bars-for-trial-safety-review
title: Prefer a table over a stacked bar chart for trial safety review
bibliography: references.bib
description: For safety-review comparison tasks on grouped treatment-outcome data,
  prefer a table over a bar chart to improve detection fidelity and mitigate missed
  adverse-event associations for domain experts.
labels:
- purpose:select
- basis:empirical
- task:compare
- chart:table:use
- chart:bar:avoid
- quality:fidelity
- lever:chart-family
- operator:association
- audience:domain-expert
---

## Table instead of stacked bar <!-- role: advice -->

Choose a table instead of a stacked bar chart when clinicians must judge whether adverse outcomes are concentrated in one treatment group. For example, show treatment-by-outcome counts in rows and columns rather than stacking the outcomes into bars for a stop-or-continue safety review.

## Why the table supports the safety decision better <!-- role: reason -->

A table makes the treatment-outcome counts directly inspectable. That supports a clearer read of whether one treatment is associated with a worse outcome pattern.

**Mechanism:** The table exposes the cross-classified counts needed for the safety judgment directly, while the stacked bar requires more visual inference about the association.

**Evidence:** The review reports that, in a simulated patient-safety review using clinical-trial adverse-event data, physicians were more likely to halt the trial when the data were shown in tables than in stacked bar charts [@anckerRethinkingHealthNumeracy2007].

## Use when reviewers must judge treatment-outcome association <!-- role: context -->

- **User Goal:** Decide whether a safety signal is strong enough to stop or flag a trial.
- **Task:** Compare outcomes across treatment groups for a strong adverse-event association.
- **Data:** Grouped treatment-by-outcome counts.
- **Chart Setting:** A static display used in clinical safety review.
- **Audience:** Physicians or other clinical reviewers.
- **Success Criterion:** More reliable detection of the adverse-event pattern that matters for the decision.

## Do not use outside this decision setting <!-- role: exceptions -->

**Break it when:** The display is not being used for clinician review of grouped treatment-outcome safety data. **Why:** The reported advantage is specific to that review setting.

## Tradeoff of replacing the stacked bar <!-- role: costs -->

**Sacrifice:** You give up the stacked bar's single combined mark.
**Risk:** If reviewers must infer the association from stacked segments, a strong safety signal can be missed.
**Mitigation:** Put the treatment and outcome counts directly into table cells.

## Common failure in safety-review displays <!-- role: mistakes -->

**Mistake:** Using a stacked bar chart for the stop-or-continue safety decision. **Why it fails:** The treatment-outcome association is harder to judge directly.

## Check the chart-family choice <!-- role: check -->

**Failure Sign:** Reviewers must estimate the association from segment sizes instead of reading counts directly.
**Quick Check:** Mock up the same data as a table and as a stacked bar chart, then ask which version makes the adverse concentration in one treatment group easier to judge directly.
**Stronger Test:** Ask a domain reviewer whether they would halt the trial from each version and treat disagreement as a sign to prefer the table.

## Fix the safety-review display <!-- role: fix -->

- Replace the stacked bar chart with a treatment-by-outcome table.
- Move the outcome counts out of stacked segments and into cells.
- Limit the display to the treatment and outcome breakdown needed for the safety decision.
