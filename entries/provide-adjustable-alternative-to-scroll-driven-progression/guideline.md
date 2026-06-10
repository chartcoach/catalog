---
id: provide-adjustable-alternative-to-scroll-driven-progression
title: Provide an adjustable alternative to scroll-driven progression
bibliography: references.bib
description: For dynamic interactive reading, use adjustable or optional progression
  controls on scroll-driven visualization sequences to improve accessibility and mitigate
  scroll-only navigation for keyboard-only users and people affected by motion or
  cognitive load.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- temporal-pattern:dynamic
- needs:keyboard-only
- access:keyboard:use
- access:motion-safe:use
---

## Add an alternative progression control <!-- role: advice -->

Add a user-controlled alternative to scroll-driven progression, and let users turn the scrolling behavior off or adjust it. For example, replace infinite scrolling, parallax scrolling, or scrollytelling with an optional "load more" or "next" control that works for keyboard-only use.

## Why adjustable progression helps <!-- role: reason -->

Scroll-driven updates can force readers through content with one input pattern and can keep motion active even when they need a calmer or more deliberate pace. A discrete alternative lets readers advance the sequence intentionally instead of depending on continuous scrolling.

**Mechanism:** Adjustable or optional progression reduces reliance on scrolling as the only interaction path and gives readers direct control over when content changes.

**Evidence:** Chartability states that scrolling experiences must be adjustable or optional and specifically names infinite scrolling, parallax scrolling, and scrollytelling, with a "load more" or "next" option in place for keyboard-only users [@elavskyHowAccessibleMy2022]. Inclusive Design Principles recommends letting users pause, stop, or adjust long-running changes and turn off features like infinite scrolling to reduce motion sickness and cognitive load [@inclusivedesignprinciples_give_control_2].

## When scroll-driven stories need a fallback <!-- role: context -->

- **User Goal:** Read or navigate a visualization sequence at a controllable pace.
- **Chart Setting:** The visualization changes as the page scrolls, such as in infinite scrolling, parallax scrolling, or scrollytelling.
- **Audience:** Includes keyboard-only users and users affected by motion or cognitive load.
- **Success Criterion:** The full sequence can be advanced without relying on continuous scrolling, and the scrolling behavior can be turned off or adjusted.

## When not to apply this rule <!-- role: exceptions -->

**Break it when:** The visualization does not use a scrolling experience or scrolling input control. **Why:** There is no scroll-driven behavior to adjust, turn off, or replace.

## Tradeoffs of alternative progression <!-- role: costs -->

**Sacrifice:** You give up automatic continuous progression as the only way the sequence advances.\
**Risk:** Adding a fallback control but keeping the scroll behavior as the only practical path still leaves the experience scroll-dependent.\
**Mitigation:** Use the same sequence with explicit user-triggered controls such as "load more" or "next," or provide a way to turn the scrolling behavior off.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep infinite scrolling, parallax scrolling, or scrollytelling as the only way to move through the visualization. **Why it fails:** Users cannot adjust or opt out of the scrolling behavior, and keyboard-only users do not get a discrete alternative control.

## How to review progression controls <!-- role: check -->

**Failure Sign:** Content changes only when the reader scrolls, and there is no visible way to turn that behavior off, adjust it, or bypass it.\
**Quick Check:** Look for an explicit alternative control such as "load more" or "next" whenever scrolling advances the content.\
**Stronger Test:** Try to move through the full sequence with keyboard-only input and confirm that all content can be reached without relying on continuous scrolling.

## How to repair scroll-only progression <!-- role: fix -->

- Add a visible control that turns off or adjusts the scroll-driven behavior.
- Replace automatic infinite scrolling with a user-triggered "load more" control.
- Replace scroll-triggered narrative steps with a user-triggered "next" control for keyboard-only use.
