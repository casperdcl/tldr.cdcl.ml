---
title: AI Bill of Rights
src: https://www.whitehouse.gov/ostp/ai-bill-of-rights
categories: [Law, Programming]
tags: [principles, law, security, ai, extra-long]
---

Principles to limit data misuse & automation from causing (unintentional) harm or infringing on civil rights.

1. [Safe & Effective Systems](https://www.whitehouse.gov/ostp/ai-bill-of-rights/safe-and-effective-systems-3)
   - consult diverse stakeholders & domain experts
   - conduct pre-deployment tests, risk identification & mitigation, monitoring
   - have independent evaluation/reporting
   - *halting deployment* should always be an option
2. [Algorithmic Discrimination Protections](https://www.whitehouse.gov/ostp/ai-bill-of-rights/algorithmic-discrimination-protections-2)
   - equitable design: should not contribute to existing societal prejudice/discrimination
   - proactive testing & independent monitoring as per (1) above
3. [Data Privacy](https://www.whitehouse.gov/ostp/ai-bill-of-rights/data-privacy-2)
   - data collection should meet "reasonable expectations"
   - data collected should be minimal ("strictly necessary")
   - users should have control ("agency") over the use of their data
     + ask for, respect, and allow user changes to consent
     + provide user with monitoring & privacy impact reports
   - {% glossary UX %}/design should not obfuscate user choice
   - explanations should be brief, in plain language, and give context/reason
   - default settings shouldn't be privacy-invasive
   - no unchecked (without diverse consultation/oversight) surveillance
   - no continuous surveillance in areas likely to reduce rights/opportunities/access (e.g. education, work, housing)
4. [Notice & Explanation](https://www.whitehouse.gov/ostp/ai-bill-of-rights/notice-and-explanation)
   - make all users aware (in plain language) that a partially/fully automated system is being used; **how** & **why** it impacts them
   - notify about key changes to functionality
   - meta-reporting: clarity & quality assessments (of notices/explanations) should be public
5. [Human Alternatives, Consideration, & Fallback](https://www.whitehouse.gov/ostp/ai-bill-of-rights/human-alternatives-consideration-and-fallback)
   - should have opt-out option
   - should have timely (accessible, maintained) human referral option
   - extra oversight for sensitive domains (e.g. criminal justice, employment, education, health)
   - public reports of above (including e.g. response times, outcomes, effectiveness)

## personal opinions

- Like all good laws, the above is lightweight and thus mostly watertight (i.e. "do not contribute to prejudice" rather than "must magically reduce prejudice").
- There are some loopholes: one-off (non-continuous) checked surveillance data can be used to manually (non-algorithmically) discriminate without violating the above. Presumably this would be caught under pre-AI discriminatory laws.
- The weakest link is likely the "diversity" of oversight.
- The title is exceedingly misleading: the focus is more on vendor *responsibilities* rather than (customer) *rights*, and on *data handling* & human-in-the-loop *monitoring of automated systems* rather than {% glossary AI %} *per&nbsp;se*.
