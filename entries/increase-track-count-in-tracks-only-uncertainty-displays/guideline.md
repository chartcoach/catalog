---
id: increase-track-count-in-tracks-only-uncertainty-displays
title: Increase track count when tracks alone must convey uncertainty
bibliography: references.bib
description: For risk judgments from uncertain geospatial paths over ordered time,
  use more than 15 visible trajectories on unannotated track displays to improve fidelity
  and mitigate underreading of spatial spread for viewers with low domain knowledge.
labels:
- purpose:refine
- basis:empirical
- time:ordered-time
- data:geospatial
- lever:layout-structure
- operator:uncertainty
- knowledge:low
- quality:fidelity
---

## Track count in tracks-only displays <!-- role: advice -->

Increase the number of visible trajectories when a path display uses tracks alone to communicate uncertainty. For example, in an unannotated forecast map, show 63 trajectories rather than 7 or 15 so viewers can better see that the spread widens later in the forecast.

## Why higher track count works in tracks-only displays <!-- role: reason -->

When a display has no attribute annotations, viewers must infer uncertainty entirely from the spatial spread of the paths. Too few visible tracks keep attention on the center and make later-time widening hard to see.

**Mechanism:** More visible paths make the forecast’s sideways spread more apparent, so readers become less anchored on the middle track and interpret later forecasts as more spatially uncertain.

**Evidence:** In the paper’s experiment, damage judgments from a 63-track unannotated display showed a flatter distance-to-damage relationship at 48 hours than at 24 hours, which matches the wider spread of the forecast. The 7-track and 15-track unannotated displays did not show this change, leading the authors to conclude that more than 15 unannotated tracks were needed and that 63 tracks worked well [@liuVisualizingUncertainTropical2019].

## When to increase track count <!-- role: context -->

- **User Goal:** Estimate risk or likely damage from the spatial spread of possible paths.
- **Task:** Read uncertainty from the path pattern itself rather than from explicit uncertainty glyphs or annotations.
- **Data:** An ensemble of possible geospatial trajectories over multiple forecast times.
- **Chart Setting:** An unannotated tracks-only display where forecast size and intensity are not encoded on the paths.
- **Audience:** Viewers with low prior domain knowledge.
- **Success Criterion:** Later-time forecasts are interpreted as more spatially spread out than earlier-time forecasts.

## When higher track count is not the right fix <!-- role: exceptions -->

**Break it when:** The display already adds size and intensity annotations to representative tracks. **Why:** In the study, annotation changed judgments enough that a 15-track annotated display outperformed a much denser unannotated display.

## Costs of higher track count <!-- role: costs -->

**Sacrifice:** You give up some spacing and visual cleanliness.
**Risk:** Adding many trajectories can create enough overdraw to make later annotation or detailed reading harder.
**Mitigation:** If you need to keep track count low, add explicit size and intensity annotations instead of leaving the display tracks-only.

## Common track-count mistake <!-- role: mistakes -->

**Mistake:** Showing only 7 or 15 unannotated tracks and expecting viewers to perceive the increase in uncertainty over time. **Why it fails:** Those displays did not produce the later-time spread reading seen with the denser 63-track display.

## How to check track count <!-- role: check -->

**Failure Sign:** Readers stay centered on the middle track at later forecast times and treat 24-hour and 48-hour forecasts as similarly concentrated.
**Quick Check:** Compare a 15-track and a 63-track version of the same unannotated display; if the denser version makes the later-time spread clearly wider, prefer it.
**Stronger Test:** Ask viewers to rate risk at equal offsets from the center track at early and late forecast times; later-time ratings should fall off less steeply when the display conveys widening spread effectively.

## How to fix low track count <!-- role: fix -->

- Increase the number of displayed trajectories above 15 when the display is tracks-only.
- Redraw the display using a denser representative subset rather than reusing the same few tracks.
- Check whether the widening spread later in the forecast becomes visible after the increase.
- If the denser display becomes too cluttered, switch to annotated representative tracks instead of staying tracks-only.
