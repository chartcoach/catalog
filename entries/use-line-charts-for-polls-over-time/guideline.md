---
id: use-line-charts-for-polls-over-time
title: Use a line chart to show poll movement over time
bibliography: references.bib
description: For trend comparison across ordered time, use a line chart instead of
  a bar chart on repeated poll series to improve insight and mitigate snapshot-only
  summaries for readers following campaign movement.
labels:
- purpose:select
- basis:heuristic
- task:trend
- time:ordered-time
- chart:line:use
- chart:bar:avoid
- quality:insight:use
- lever:chart-family
---

## Use the time-series chart <!-- role: advice -->

Choose a line chart when the chart’s job is to show how poll support changes across dates. For example, plot each party as a line across months and use that view rather than a latest-poll bar chart when the story is about movement during the campaign or since the last election.

## Why the time-series chart works <!-- role: reason -->

A line chart keeps the date sequence visible, so readers can follow rises, declines, and crossings as trajectories instead of isolated values.

**Mechanism:** The connected time axis turns repeated poll readings into movement, which makes change over time readable in one view.

**Evidence:** The post presents the line chart as the common lead visualization for polls over time, with examples spanning either one campaign year or multiple election cycles, and contrasts that use with bar or column charts for latest-poll snapshots [@muth_german_election_2021].

## Use when the story is about movement <!-- role: context -->

- **User Goal:** Show how support changed during a campaign or across election cycles.
- **Task:** Compare trajectories across parties.
- **Data:** Repeated poll values collected at multiple dates.
- **Chart Setting:** One chart is meant to summarize a time path, not just the newest estimate.
- **Success Criterion:** Readers can see when support rises, falls, or changes direction over time.

## Do not use when only the newest estimate matters <!-- role: exceptions -->

**Break it when:** The chart only needs to show the latest poll, an average of the latest polls, or a forecast at one moment. **Why:** The post treats that as a snapshot task better served by a bar or column chart.

## Tradeoffs of the time-series chart <!-- role: costs -->

**Sacrifice:** A line chart gives less emphasis to one newest snapshot.
**Risk:** If the article is only about the current estimate, the time path can distract from that single-date comparison.
**Mitigation:** Switch to a bar or column chart when the latest estimate is the only point that matters.

## Common failure around the time-series chart <!-- role: mistakes -->

**Mistake:** Use a latest-poll bar chart for a story about campaign movement. **Why it fails:** The bar view removes the month-to-month path that the line chart is meant to preserve.

## Check whether the chart needs time structure <!-- role: check -->

**Failure Sign:** The story talks about changes across months or years, but the chart only shows one bar per party.
**Quick Check:** Compare a quick line-chart sketch against a latest-poll bar sketch; if only the line preserves the rise-and-fall pattern, choose the line chart.
**Stronger Test:** Ask whether a reader can tell how support changed across the period from the graphic alone.

## Fix the snapshot mismatch <!-- role: fix -->

- Replace the snapshot bars with one line per series across dates.
- Keep the dates on the horizontal axis so the time order is explicit.
- If you truly have only one current estimate, drop the line chart and use a bar or column chart instead.
