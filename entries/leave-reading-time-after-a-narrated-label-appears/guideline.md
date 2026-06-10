---
id: leave-reading-time-after-a-narrated-label-appears
title: Leave reading time after a narrated label appears
bibliography: references.bib
description: For ordered-time narrated visuals, avoid new motion or reveals during
  label-reading intervals on dynamic displays to improve readability and mitigate
  missed labels for viewers learning unfamiliar terms.
labels:
- purpose:refine
- basis:empirical
- time:ordered-time
- temporal-pattern:dynamic
- quality:readability:use
- lever:text-annotation
- component:label:use
---

## Hold the screen for label reading <!-- role: advice -->

Keep the display stable long enough for viewers to read a cued label. For example, reveal the label when narration names it, then delay the next reveal or animation until that label can be read.

## Why label reading time matters <!-- role: reason -->

A label competes badly with a new motion event. If animation starts while the viewer is trying to read the named label, attention shifts away before the object-label link is formed.

**Mechanism:** A spoken label cue creates a short interval when viewers need to read and connect the label to the object. New motion or reveals in that same interval pull attention away.

**Evidence:** The paper recommends allowing reading time after cueing a label and avoiding reveals or animation during the speech segment that cues it; in the studied sequence, rapid motion and competing animation caused some labels or actions to be missed [@faradayDesigningEffectiveMultimedia1997].

## Use when labels introduce unfamiliar terms <!-- role: context -->

- **User Goal:** Read and retain the name of an on-screen object during a process explanation.
- **Data:** The display introduces new labels over time.
- **Chart Setting:** A narrated dynamic display could start another reveal or animation immediately after a label appears.
- **Audience:** Viewers may not already know the terminology.
- **Success Criterion:** Viewers can read the label and connect it to the right object before the next step begins.

## Do not add a pause when there is no new label to read <!-- role: exceptions -->

**Break it when:** No newly cued label appears in that interval. **Why:** This recommendation is specifically about the reading window created when narration introduces a label.

## What reading time costs <!-- role: costs -->

**Sacrifice:** You give up some pace.
**Risk:** The sequence can feel slower if every step pauses equally.
**Mitigation:** Reserve the pause for labels and terms that viewers must identify.

## Common label-timing misuse <!-- role: mistakes -->

**Mistake:** Starting a new animation as soon as a label appears. **Why it fails:** Attention shifts to the motion before the label is read.

## How to test label timing <!-- role: check -->

**Failure Sign:** Viewers remember the moving event but cannot name the labeled item.
**Quick Check:** For each spoken label, check whether another reveal or animation starts before the cue finishes.
**Stronger Test:** Show the segment once and ask viewers to name the labeled item immediately afterward.

## What to change <!-- role: fix -->

- Delay the next animation until the label cue finishes.
- Keep the labeled object and its label stable during the spoken term.
- Slow or pause a moving element that would otherwise compete with the label.
- Remove overlapping reveals from the same interval.
