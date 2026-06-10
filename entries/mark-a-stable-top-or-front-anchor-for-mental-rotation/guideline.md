---
id: mark-a-stable-top-or-front-anchor-for-mental-rotation
title: Mark a stable top or front anchor when readers must mentally rotate a structure
bibliography: references.bib
description: For mental-rotation tasks on multi-part object diagrams, use a persistent
  top or front marker on the object to improve fidelity and mitigate ambiguous rotation
  framing for readers interpreting rotated structures.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity
- lever:encoding
- component:annotation:use
- polish:focus
---

## Persistent top/front marker <!-- role: advice -->

Add one persistent top or front marker to the rotated object. For example, highlight the top part or add an arrowhead-like cue that stays attached to the same part so readers can compute clockwise or counterclockwise change from one stable reference.

## Why one anchor helps rotation <!-- role: reason -->

Mental rotation in this task worked through a single tracked part rather than through a fully detailed whole-object image. A stable top/front anchor gives readers the same single reference point that attention naturally selects and follows.

**Mechanism:** One spotlight of attention can keep one part “glued” to its position during rotation. Marking that part externally reduces ambiguity about which point defines the object’s orientation and rotation direction.

**Evidence:** In mental rotation, feature-binding capacity dropped to about one item, swap detection was much better when the top part was involved, and eye tracking showed that readers usually selected and tracked the topmost part through the imagined rotation [@xuCapacityVisualFeatures2015].

**Notes:** The paper explicitly links improved mental rotation to cues that provide an axis “arrowhead” or object “front.”

## Use when rotation must be imagined <!-- role: context -->

- **User Goal:** Judge whether two views show the same object after a rotation.
- **Data:** A multi-part object with distinct features attached to different parts.
- **Chart Setting:** A diagram or instructional graphic where the rotated state is not shown directly and readers must infer clockwise or counterclockwise change.
- **Audience:** Readers doing spatial reasoning with structured objects.
- **Success Criterion:** Readers preserve the correct orientation and feature-to-part mapping through the rotation step.

## Do not use for static or scaling tasks <!-- role: exceptions -->

**Break it when:** The object stays static or the required transformation is scaling rather than rotation. **Why:** The paper found much less disruption to feature-part binding in no-rotation and scaling conditions, so a top/front anchor is not the main bottleneck there.

## Tradeoffs of a stable anchor <!-- role: costs -->

**Sacrifice:** You give one part privileged visual status.
**Risk:** Readers may over-focus on the anchor and neglect other parts.
**Mitigation:** Keep the anchor stable and singular, and use it specifically to support the rotation step.

## Competing anchors <!-- role: mistakes -->

**Mistake:** Marking several different parts as directional references or changing which part counts as the front across views. **Why it fails:** The evidence points to a single tracked reference, so competing anchors remove the stable point readers need.

## Review the anchor cue <!-- role: check -->

**Failure Sign:** Readers make clockwise/counterclockwise errors or disagree about which side of the object is the front.
**Quick Check:** Ask a reviewer to point to the object's top/front before describing the rotation.
**Stronger Test:** Compare rotation judgments with and without the persistent top/front marker.

## Edits that add one anchor <!-- role: fix -->

- Highlight one part as the object's top or front.
- Keep that same part marked across all rotated states.
- Remove extra directional cues that point to different parts.
