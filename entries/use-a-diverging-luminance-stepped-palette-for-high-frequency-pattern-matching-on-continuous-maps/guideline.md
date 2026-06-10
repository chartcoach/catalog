---
id: use-a-diverging-luminance-stepped-palette-for-high-frequency-pattern-matching-on-continuous-maps
title: Use a diverging luminance-stepped palette for high-frequency pattern matching
  on continuous maps
bibliography: references.bib
description: For spatial profile matching on high-spatial-frequency continuous maps,
  prefer a diverging palette with stepped luminance on a color-encoded map to improve
  pattern discrimination and mitigate missed fine-grained features for viewers matching
  patterns across space.
labels:
- purpose:refine
- basis:empirical
- task:trend
- chart:map
- quality:fidelity:use
- lever:encoding
- aesthetic:color:use
---

## Diverging luminance-stepped palette for pattern matching <!-- role: advice -->

Use a diverging luminance-stepped palette when the map must support matching fine-grained spatial patterns. For example, on a high-spatial-frequency map, replace rainbow or the tested sequential and spiral ramps with a coolwarm-like or spectral-like diverging ramp when readers need to match the profile between two locations.

## Why stepped diverging luminance helps pattern matching <!-- role: reason -->

Pattern matching in complex maps depended on color design. Only the diverging palettes with stepped luminance reliably improved profile-matching success as spatial frequency increased.

**Mechanism:** A diverging ramp with stepped luminance makes small rises, falls, and turning points easier to distinguish when readers must extract and match a profile from the map.

**Evidence:** In the collated high-frequency pattern-matching result, E-6 ranked first and E-7 ranked second, and both significantly outperformed E-1, E-2, E-3, E-5, and E-9; the paper recommends these diverging ramps for high-spatial-frequency pattern perception and warns against rainbow, sequential, and spiral schemes for fine-grained feature analysis in complex maps [@zengReviewCollationGraphical2023; @redaGraphicalPerceptionContinuous2018].

## Use when readers must match a fine-grained spatial profile <!-- role: context -->

- **User Goal:** Match the shape of a spatial profile between two points.
- **Task:** Pattern or profile matching on a continuous surface.
- **Data:** Continuous quantitative data with high spatial frequency and fine-grained local structure.
- **Chart Setting:** A static pseudocolor map where readers compare the map to an external profile or candidate patterns.
- **Audience:** Viewers interpreting detailed spatial patterns from color alone.
- **Success Criterion:** More correct matches between the map-derived profile and the candidate pattern.

## Do not use when the surface is smooth or the task is exact lookup <!-- role: exceptions -->

**Break it when:** The field is low-spatial-frequency or the main task is exact value lookup at specific locations. **Why:** Low-frequency pattern matching showed no clear palette advantage, and exact lookup favored a different palette strategy.

## Costs of a pattern-specific palette choice <!-- role: costs -->

**Sacrifice:** You optimize for fine-grained pattern perception rather than for exact value lookup.
**Risk:** Reusing a lookup-oriented palette such as rainbow on a complex pattern-reading task can reduce or fail to improve profile-matching success.
**Mitigation:** Reserve this palette family for maps whose main job is fine-grained pattern or profile interpretation.

## Common pattern-matching failure <!-- role: mistakes -->

**Mistake:** Keeping rainbow or a tested sequential or spiral ramp on a complex map whose main job is profile matching. **Why it fails:** Those palettes were associated with lower or unreliably improved success in high-spatial-frequency pattern tasks.

## Check profile matching with a direct palette comparison <!-- role: check -->

**Failure Sign:** Readers frequently pick the wrong candidate pattern for the same marked path.
**Quick Check:** Show the same high-frequency map with the current palette and with a diverging luminance-stepped palette, then ask readers to match the marked profile; keep the version with more correct matches.
**Stronger Test:** Repeat the profile-matching check across several high-frequency maps before standardizing the palette.

## Fix the pattern-matching palette <!-- role: fix -->

- Replace rainbow or a tested sequential or spiral ramp with a diverging luminance-stepped ramp on the same complex map.
- Test a coolwarm-like diverging ramp and a spectral-like diverging ramp against the current palette using the same marked profile.
- Keep the palette that improves correct profile matches on high-spatial-frequency fields.
- If the map’s main job changes to exact value lookup, re-test with a lookup-oriented hue-varying palette instead.
