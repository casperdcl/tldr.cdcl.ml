---
title: Open Source is Illegal
src: https://talks.cdcl.ml/os-is-illegal
categories: [Programming, Industry, Law]
tags: [opinionated, principles, law, oss, security, extra-long]
---

We might be accidentally fighting on behalf of worst-offending profiteering companies.

- :lock_with_ink_pen: not all terms in (software) licences are legally binding
  + only [rare cases involving lots of money](https://www.theregister.com/2023/06/09/github_copilot_lawsuit) go to court
  + "[it is a necessary condition of a [...] law that it should be enforceable](https://doi.org/10.2307/2214413)" which is infeasible with most current software
  + law cannot address both fraud/profiteering & indecency/rudeness (too broad scope)
- :scroll: recap of [*Open Source is Bad*]({% post_url 2023-04-18-os-is-bad %}):
  + lack of warranties in {% glossary OSS %} = deliberate & accidental errors
  + could be solved by public funding
- :hammer: instead of funding, EU have suggested cybersecurity legislation
  + [Cyber Resilience Act](https://digital-strategy.ec.europa.eu/en/library/cyber-resilience-act) & [Product Liability Act](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A52022PC0495) proposed in Sept 2022 to hold profiteering companies accountable (via "consumer interests" and "safety & liability" of products/services)
  + aim: anyone making (in)direct profit cannot hide behind "NO WARRANTY" licence clauses
  + [131 feedback submissions](https://ec.europa.eu/info/law/better-regulation/have-your-say/initiatives/13410-Cyber-resilience-act-new-cybersecurity-rules-for-digital-products-and-ancillary-services/feedback_en?p_id=31490443) + [ongoing meetings](<https://oeil.secure.europarl.europa.eu/oeil/popups/ficheprocedure.do?lang=en&reference=2022/0302(COD)>)
- :crossed_swords: cons
  + can liability traverse dependency graph (blame pushed onto {% glossary FOSS %} dependencies)?
  + could "indirect" profit include "self-promotion" and thus all FOSS?
  + :confounded: surprisingly, some non-profits like the {% glossary PSF %} [are unhappy](https://pyfound.blogspot.com/2023/04/the-eus-proposed-cra-law-may-have.html)
    * threatens to block `python` & `pip` installs in EU
    * thinks proposed law could hold individual FOSS devs unfairly accountable (personal note: huge commercial orgs with ongoing {% glossary IP %} cases against them happily [regurgitate the same arguments](https://github.blog/2023-07-12-no-cyber-resilience-without-open-source-sustainability))
- :person_fencing: rebuttal against "cons"
  + FOSS devs & non-profits are [fighting to dilute proposed laws]({% post_url 2023-04-19-CRA-PLA-cybersecurity-law-rewording-appeal %}) on behalf of worst-offending profiteering companies
  + people might be arguing without understanding prerequisite legal jargon nor seeking unbiased legal advice (most modern debates rely on media sensationalism & misunderstanding jargon)
  + could just reword a little
    * expressly (not just implicitly) exclude indie packages
  + somebody should be accountable if critical infra (e.g. {% glossary PyPI %}, [Linux]({% post_url 2022-07-24-linux-foss-warranty %})) breaks
    * if devs/orgs (e.g. PSF) aren't paid enough to provide warranties, should be given public funding (via governments/{% glossary NGO, display: NGOs %}) purely in interest of public safety
