---
id: separate-evidence-strength-from-the-action-threshold
title: Separate evidence strength from the action threshold in categorical recommendations
bibliography: references.bib
description: For action-threshold decisions, use annotations that distinguish evidence
  strength from the decision rule on categorical recommendations to improve trust
  and mitigate confusion about why the display recommends action or inaction for decision-makers.
labels:
- purpose:refine
- basis:empirical
- quality:trust:use
- lever:text-annotation
- operator:uncertainty
- component:caption:use
- communication:credibility
- audience:decision-maker
---

## Two-part recommendation annotations <!-- role: advice -->

Annotate a categorical recommendation with both the strength of the underlying evidence and the caution level of the decision rule. For example, label whether a call to act comes from strong discrimination, from a deliberately cautious threshold that accepts more false alarms, or from weak evidence paired with a precautionary rule.

## Why two-part recommendation annotations work <!-- role: reason -->

A yes/no recommendation compresses two different things into one visible outcome: how well experts can tell states of the world apart and how cautiously they choose to act on that evidence. When the display separates those parts, readers can judge the recommendation without confusing uncertainty in the science with the values built into the threshold.

**Mechanism:** Distinguishing evidence strength from threshold choice helps readers understand why a recommendation was made and reduces mistrust when outcomes later make the recommendation look overly cautious or insufficiently cautious.

**Evidence:** The paper argues that categorical advice always reflects both discrimination ability and the decision rule, shows that failure to communicate both can lead to misinterpretation and distrust, and recommends making the uncertainties underlying recommendations transparent [@fischhoffCommunicatingScientificUncertainty2014].

## When to use two-part recommendation annotations <!-- role: context -->

- **User Goal:** Decide whether to act now or not act yet.
- **Task:** Interpret a categorical recommendation that crosses an action threshold.
- **Chart Setting:** The display ends in a call such as act/do not act, transfer/do not transfer, treat/do not treat, or buy/sell.
- **Audience:** Readers are evaluating advice rather than inspecting the full underlying evidence themselves.
- **Success Criterion:** Readers can tell whether the recommendation reflects strong evidence, a cautious threshold, or both.

## When not to use two-part recommendation annotations <!-- role: exceptions -->

**Break it when:** The display is not making a categorical action recommendation and instead leaves the choice among fixed options to the reader. **Why:** The paper treats this distinction as specific to threshold-triggered decisions.

## Tradeoffs of two-part recommendation annotations <!-- role: costs -->

**Sacrifice:** You give up the simplicity of a bare yes/no call.
**Risk:** Extra explanation can clutter a compact display.
**Mitigation:** Use a short paired note that separately states evidence strength and threshold rationale.

## Common failure with two-part recommendation annotations <!-- role: mistakes -->

**Mistake:** Showing only the categorical recommendation with no explanation of confidence or threshold. **Why it fails:** Readers may blame the wrong source of error and misjudge what experts know versus how cautiously they chose to act.

## How to check two-part recommendation annotations <!-- role: check -->

**Failure Sign:** Viewers can repeat the recommendation but cannot say why it was made.
**Quick Check:** Can a reviewer point to one statement about evidence strength and a separate statement about the action threshold or tradeoff?
**Stronger Test:** Ask intended readers whether the recommendation reflects knowledge limits, a cautious rule, or both, and compare their answers with the display’s intended message.

## How to fix two-part recommendation annotations <!-- role: fix -->

- Add a short caption sentence stating the strength of the underlying evidence.
- Add a second sentence stating the threshold rationale or tradeoff behind the recommendation.
- Separate “what the evidence supports” from “how cautious the rule is” in any legend, note, or boxed summary.
- Expand a one-line recommendation into a two-line explanation when the recommendation would otherwise hide this distinction.
