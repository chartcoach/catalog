---
id: make-customized-chart-state-easy-to-share-and-reproduce
title: Make customized chart state easy to share and reproduce
bibliography: references.bib
description: For distributing results from exploratory interaction, use shareable
  saved state on interactive charts and dashboards to improve accessibility and mitigate
  manual reconstruction or screenshot-only sharing for analysts sharing customized
  views with others.
labels:
- purpose:refine
- basis:accessibility
- task:distribute
- quality:accessibility
- lever:interaction-access
- communication:workflow
- audience:analyst
---

## Shareable saved state <!-- role: advice -->

Preserve the current chart state in a shareable artifact that reopens the same view. For example, let a customized dashboard view be shared through one link, file, or saved state so another person sees the same parameters instead of recreating the interaction path or relying on a screenshot.

## Why shareable state works <!-- role: reason -->

Preserving the current state lets a discovered view travel with the analysis. Readers can reopen the exact result instead of repeating a branching interaction sequence, which reduces cognitive work and keeps the evidence inside the interactive system rather than collapsing it into a static image.

**Mechanism:** A shareable saved state removes the need to remember and repeat the steps that produced a customized view. It also avoids screenshot handoffs that separate the finding from the live chart state.

**Evidence:** Chartability identifies hard-to-share customized views as an accessibility barrier in complex dashboards and exploratory applications because others must reproduce the analysis themselves or fall back to screenshots, which add cognitive effort and accessibility risk [@elavskyHowAccessibleMy2022]. Preserving exact view parameters in a shareable URL or report-sharing flow is a concrete way to recreate the same state for another viewer [@moz_everything_you; @key2consulting_how_share].

**Notes:** The requirement applies when interaction changes the current view in a meaningful way.

## When to apply this <!-- role: context -->

- **User Goal:** Share a specific finding discovered in a customized view.
- **Task:** Distribute or hand off an exploratory result without re-explaining each interaction step.
- **Chart Setting:** An interactive chart, dashboard, or branching narrative where user actions produce a non-default view.
- **Audience:** Another analyst or viewer who needs to reopen the same view.
- **Success Criterion:** One link, file, or saved state reproduces the same chart state for the next viewer.

## When not to apply this <!-- role: exceptions -->

**Break it when:** The chart has no customized state and no interaction that changes the current view. **Why:** There is no non-default view to preserve or reproduce.

## Tradeoffs of shareable state <!-- role: costs -->

**Sacrifice:** The shared artifact must carry the current interaction state instead of only showing the default chart.
**Risk:** If the shared artifact does not preserve the exact current parameters, the recipient will not see the same view.
**Mitigation:** Encode or save the full current state in one link, file, or saved state.

## Common failure modes <!-- role: mistakes -->

- **Mistake:** Making people recreate the view by repeating the interaction path. **Why it fails:** It adds significant cognitive effort and turns sharing into a usability barrier.
- **Mistake:** Sharing only a screenshot of the customized view. **Why it fails:** It loses the proof in the system and creates a new accessibility risk.

## How to review it <!-- role: check -->

**Failure Sign:** A useful non-default view can only be shared with screenshots or step-by-step instructions.
**Quick Check:** Create a customized view and ask whether one link, file, or saved state can reopen it.
**Stronger Test:** Open the shared artifact in a fresh session and confirm it shows the same customized view without extra setup.

## How to fix it <!-- role: fix -->

- Add a share action that captures the current chart state in one link.
- Add save or export support that reopens the same customized view from one file or saved state.
- Persist the exact current parameters of the interaction so the recipient sees the same non-default view on open.
- Replace screenshot-only sharing paths with live state sharing for exploratory findings.
