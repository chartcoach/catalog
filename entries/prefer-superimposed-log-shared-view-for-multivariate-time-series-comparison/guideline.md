---
id: prefer-superimposed-log-shared-view-for-multivariate-time-series-comparison
title: Prefer a superimposed log-scaled shared view for multivariate time-series comparison
bibliography: references.bib
description: For comparison tasks on ordered time, prefer a superimposed log-scaled
  shared view on multivariate line charts to improve comparison speed and mitigate
  slow cross-row reading for readers comparing several series.
labels:
- purpose:select
- basis:empirical
- task:compare
- time:ordered-time
- structure:single-view:use
- structure:small-multiples:avoid
- measure:multi
- quality:readability:use
- lever:layout-structure
---

## Use a shared comparison view <!-- role: advice -->

Use a superimposed log-scaled shared view when readers need to compare multiple time series quickly. For example, replace a row-separated linear line-plot layout with one shared line plot on a log-scaled y-axis, and keep color hue to distinguish the overlaid series.

## Why the shared log view is faster <!-- role: reason -->

A shared view keeps the lines close together, so readers can compare them directly instead of scanning across separate rows. In this contrast, the improvement is about speed, not a measured gain in correctness.

**Mechanism:** Superimposition reduces cross-row comparison work, and the tested shared log view supported faster answers on cross-series comparison tasks.

**Evidence:** In the collated extraction, the superimposed log-scaled line plot ranked above the row-separated linear line plot for correlate, aggregate, and overall time, with significant pairwise differences, while the corresponding accuracy contrasts showed no significant pairwise difference [@zengReviewCollationGraphical2023; @aignerBertinWasRight2011].

**Notes:** The supported finding is the tested whole-view contrast, not an isolated claim about log scaling alone.

## Use when comparing multiple time series <!-- role: context -->

- **User Goal:** Compare several time series quickly.
- **Task:** Judge cross-series correlation or aggregate behavior.
- **Data:** Multiple ordered-time series shown together.
- **Chart Setting:** A line-chart choice between a row-separated linear layout and a superimposed log-scaled shared view.
- **Audience:** Readers performing visual comparison across several series.
- **Success Criterion:** Shorter task completion time.

## Do not use when accuracy is the only goal <!-- role: exceptions -->

**Break it when:** The main success criterion is improved correctness rather than faster completion. **Why:** The tested contrast showed a time advantage for the superimposed log view, but not a significant accuracy advantage.

## Tradeoffs of the shared log view <!-- role: costs -->

**Sacrifice:** You give up the row-separated linear arrangement.
**Risk:** The switch can be overclaimed as an accuracy improvement even though the measured difference was in time.
**Mitigation:** Use this contrast when faster comparison is the target outcome and review it with the same task type you expect readers to perform.

## Common layout failure <!-- role: mistakes -->

**Mistake:** Keep multivariate time series in separate rows on a linear scale for correlation or aggregate comparison. **Why it fails:** The tested row-separated linear view took longer than the superimposed log-scaled shared view on the same task types.

## Compare the two layouts directly <!-- role: check -->

**Failure Sign:** Readers are slow when answering cross-series correlation or aggregate questions.
**Quick Check:** Build two versions of the same line chart: one row-separated with a linear y-axis and one superimposed with a log y-axis, then compare answer times on the same questions.
**Stronger Test:** Time a short set of correlation and aggregation tasks on both versions and keep the version with consistently shorter completion times.

## Change the layout and scale <!-- role: fix -->

- Remove the row separation and place the series in one shared line plot.
- Switch the shared y-axis from linear to log.
- Keep color hue to differentiate the overlaid lines after superimposition.
- Re-test the revised chart against the row-separated linear version on the same comparison tasks.
