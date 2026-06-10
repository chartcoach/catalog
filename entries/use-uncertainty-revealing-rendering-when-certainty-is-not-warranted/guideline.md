---
id: use-uncertainty-revealing-rendering-when-certainty-is-not-warranted
title: Use uncertainty-revealing rendering when certainty is not warranted
bibliography: references.bib
description: For uncertainty communication in quantitative displays, use uncertainty-revealing
  rendering on charts to improve trust and mitigate false objectivity for readers.
labels:
- purpose:refine
- basis:empirical
- operator:uncertainty
- lever:encoding
- communication:credibility
- quality:trust:use
- aesthetic:style:use
---

## Uncertainty-revealing rendering <!-- role: advice -->

Add rendering that visibly signals tentativeness when the data should be questioned. For example, use sketchy drawing styles or explicit uncertainty-conveying renderings instead of a clean minimalist presentation when uncertainty, missingness, or bias is part of the message.

## Why visible uncertainty helps <!-- role: reason -->

A polished, exact-looking chart can make uncertain data feel more authoritative than it is. Visual signals of tentativeness can slow overconfident reading and make viewers more willing to question the evidence.

**Mechanism:** Clean minimalist rendering can project objectivity and certainty, while sketchy or uncertainty-revealing styling makes uncertainty part of what the reader perceives.

**Evidence:** The paper argues that clean layouts can grant unwarranted authority and objectivity to data, while sketchy and uncertainty-conveying renderings can increase willingness to critique and appreciation of uncertainty [@bertiniWhyShouldntAll2020].

## Use when the chart should not look fully settled <!-- role: context -->

- **User Goal:** Communicate uncertainty, tentativeness, or the need for critique.
- **Task:** Uncertainty communication rather than only fast value extraction.
- **Data:** Uncertain, missing, biased, or otherwise not fully settled.
- **Chart Setting:** A quantitative display that might otherwise look overly clean and authoritative.
- **Audience:** Readers who might otherwise take the chart as objective truth.
- **Success Criterion:** Readers notice uncertainty and remain willing to question the display.

## Do not use when fast exact reading is the whole job <!-- role: exceptions -->

**Break it when:** The display is meant for fast, exact reading of settled values and uncertainty is not part of the message. **Why:** The extra visual difficulty can slow decoding without adding needed information.

## Costs of uncertainty-revealing rendering <!-- role: costs -->

**Sacrifice:** You give up some speed and precision in immediate value reading.
**Risk:** Blind use can make already-clear data harder to decode.
**Mitigation:** Apply the treatment when the chart should explicitly communicate uncertainty or invite critique.

## Common certainty mistake <!-- role: mistakes -->

**Mistake:** Keeping a clean minimalist rendering when uncertainty is central to the story. **Why it fails:** The chart can look more objective and settled than the data deserves.

## Check whether the chart overstates certainty <!-- role: check -->

**Failure Sign:** Uncertain data looks fully settled and authoritative.
**Quick Check:** Remove the title and caption and ask whether the marks themselves still signal uncertainty.
**Stronger Test:** Compare a clean version and an uncertainty-revealing version; if the clean version looks more certain than the data warrants, the original is masking uncertainty.

## Fix the rendering <!-- role: fix -->

- Apply sketchy styling to the uncertain marks.
- Add explicit uncertainty-conveying rendering where values are missing or uncertain.
- Replace a purely clean minimalist treatment that hides the tentativeness of the data.
