---
id: align-relational-wording-with-highlighted-object
title: Match relational wording to the highlighted object
bibliography: references.bib
description: For ordered-time explanation of binary spatial relations, use text annotation
  on paired visual objects to improve readability and mitigate slower verification
  from cue-wording mismatches for readers interpreting left/right or above/below layouts.
labels:
- purpose:refine
- basis:empirical
- task:relate
- time:ordered-time
- quality:readability
- lever:text-annotation
- component:annotation:use
- group-cardinality:binary
---

## Align target wording to the highlighted object <!-- role: advice -->

Make the object that is highlighted or shown first the grammatical target of the relational annotation. For example, if a staged explanation shows one mark before the other for a left/right or above/below relation, name that first-seen mark first in the sentence and describe its relation to the other mark.

## Why target-aligned wording reads faster <!-- role: reason -->

A brief visual cue makes one object in a pair feel like the special object in the relation. Text that assigns that same object the target role is verified faster than text that assigns the other object the target role.

**Mechanism:** Aligning the highlighted object with the sentence target lets the same object serve as both the perceptual focus and the linguistic focus, reducing the work needed to map the display to the wording.

**Evidence:** In sentence-picture verification tasks with two objects, responses were faster when the briefly previewed object was the linguistic target rather than the reference object. This held for both left/right and above/below relations [@rothAsymmetricCodingCategorical2012].

**Notes:** The robust effect was target/reference alignment. Effects based only on the direction word were weaker and harder to interpret.

## Use when one object is made special first <!-- role: context -->

- **User Goal:** Explain or verify which of two objects is left/right or above/below the other.
- **Task:** Read a short relational statement against a staged or highlighted visual pair.
- **Data:** Two visual objects that form a simple categorical spatial relation.
- **Chart Setting:** One object is previewed, highlighted, or otherwise receives attention before the other.
- **Audience:** Readers who must quickly match the display to accompanying wording.
- **Success Criterion:** Faster verification of the depicted relation.

## Do not use for direction-only prompts <!-- role: exceptions -->

**Break it when:** The text only asks which object is on a named side or position, without assigning target and reference roles to both objects. **Why:** The paper found those simpler direction-only effects weak and hard to interpret, with possible priming from the previewed object's identity.

## Tradeoffs of target-aligned wording <!-- role: costs -->

**Sacrifice:** You give up some freedom to phrase the same relation from either object's perspective.
**Risk:** If no object is actually highlighted or shown first, forcing target-first wording may not help.
**Mitigation:** Apply the rule only when the display clearly makes one object the attentional focus before the full relation is read.

## Common wording mismatch <!-- role: mistakes -->

**Mistake:** Highlight one object first, then write the relation from the other object's perspective. **Why it fails:** The cue makes one object perceptually special, but the sentence asks the reader to treat the other object as the target.

## Check cue-text alignment <!-- role: check -->

**Failure Sign:** Readers slow down when matching the staged pair to the annotation, even though the relation is simple.
**Quick Check:** Identify which object appears first or is highlighted, then check whether that same object is named first as the target in the relation text.
**Stronger Test:** A/B test target-aligned wording against reference-aligned wording on the same two-object display and compare verification speed.

## Fix target-reference wording <!-- role: fix -->

- Rewrite the annotation so the highlighted object is the sentence target.
- If the text currently describes the opposite perspective, flip the relation to its inverse wording while keeping the same scene.
- If the wording must stay fixed, change the build or highlight order so the named target receives attention first.
