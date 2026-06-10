---
id: pair-relative-effect-claims-with-absolute-effect-summaries
title: Pair relative effect claims with absolute effect summaries
bibliography: references.bib
description: For communicating single treatment-effect results, use text annotations
  that include absolute effect summaries on quantitative result displays to improve
  fidelity and mitigate overstatement of intervention benefit for domain-expert decision
  makers.
labels:
- purpose:refine
- basis:empirical
- scope:single-result
- data:quantitative
- quality:fidelity
- lever:text-annotation
- communication:framing
- audience:decision-maker
---

## Absolute effect annotation <!-- role: advice -->

Add an absolute effect summary to the result annotation instead of leaving a relative percentage on its own. For example, pair a relative reduction with an absolute risk change stated per population and time period, or add a number-needed-to-treat statement such as how many people must be treated for a set duration to prevent one event.

## Why absolute summaries work <!-- role: reason -->

Relative percentages can make an intervention look larger because they hide the untreated baseline and the large denominator of people who do not benefit. Absolute risk changes and number-needed-to-treat summaries make readers account for baseline risk and treatment burden, which leads to more conservative judgments about benefit.

**Mechanism:** Absolute summaries change the reader's interpretation from "how large is the proportional drop?" to "how many events are actually prevented, for how many people, over what time?" That reduces inflation of perceived effectiveness when event rates are low.

**Evidence:** In a randomized survey of 499 Swiss primary care physicians, reporting preventive treatment effects as absolute risk reduction instead of relative risk reduction lowered rated effectiveness and lowered willingness to treat for myocardial infarction outcomes. Reporting number needed to treat lowered ratings even more than absolute risk reduction for the same beneficial outcome. The study found no significant difference for the total-mortality endpoint in this setting [@bucherInfluenceMethodReporting1994].

**Notes:** The paper's discussion recommends reporting actual event rates and absolute changes in risk because relative-risk-only reporting can overstate benefit.

## Use when treatment decisions depend on one summarized outcome <!-- role: context -->

- **User Goal:** Decide whether an intervention is effective enough to recommend or prescribe.
- **Task:** Interpret one reported treatment-effect summary from a trial or evidence display.
- **Data:** Quantitative event outcomes summarized as risk reductions; especially relevant when event incidence is low.
- **Chart Setting:** A chart, table, caption, or text-first result display that currently summarizes an outcome with a single effect statement.
- **Audience:** Physicians or other domain experts making treatment decisions.
- **Success Criterion:** Readers do not overestimate benefit from a relative percentage alone.

## Do not rely on this effect for outcomes like total mortality in this study <!-- role: exceptions -->

**Break it when:** The outcome matches the total-mortality case in this evidence setting. **Why:** The study did not find a significant difference in judgments between relative-risk and absolute-risk wording for that endpoint.

## Tradeoffs of absolute effect annotation <!-- role: costs -->

**Sacrifice:** The result may feel less impressive than a relative percentage alone.\
**Risk:** If you replace the relative percentage entirely, readers may lose the proportional comparison.\
**Mitigation:** Keep the relative percentage only if it is paired with the absolute effect summary rather than shown alone.

## Common framing mistake <!-- role: mistakes -->

**Mistake:** Put only a relative risk reduction in the main result annotation. **Why it fails:** That framing led physicians to rate the treatment as more effective and to be more inclined to treat than when absolute-risk or number-needed-to-treat summaries were shown.

## Check for relative-risk-only framing <!-- role: check -->

**Failure Sign:** The main takeaway is a percentage reduction with no absolute event change, denominator, or treatment count.\
**Quick Check:** Rewrite the same result as an absolute event change per population and time period, or as number needed to treat, and compare it with the current wording. If the current display only shows the relative percentage, it uses the overstating format tested in the paper.\
**Stronger Test:** A/B test the current annotation against an absolute-summary version with domain readers and compare perceived effectiveness or stated willingness to act.

## Fix the summary annotation <!-- role: fix -->

- Add an absolute risk change to the main result statement using a stated population and time period.
- Add a number-needed-to-treat annotation for the main beneficial outcome when that quantity can be stated.
- If a relative percentage remains, place it beside the absolute summary instead of presenting it alone.
