---
title: CRA & PLA Cybersecurity Laws Need Rewording
src: https://www.theregister.com/2023/04/12/python_management_eu
categories: [Programming, Industry, Law]
tags: [opinionated, principles, law, oss, security]
---

Proposed EU laws to restrict irresponsible businesses might be abused to hurt {% glossary FOSS %} volunteers due to poor wording.

- the [Cyber Resilience Act (CRA)](https://digital-strategy.ec.europa.eu/en/library/cyber-resilience-act) & [Product Liability Act (PLA)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A52022PC0495) aim to increase software security & accountability
  + [Article 16](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=celex%3A52022PC0454) states a "person, other than [manufacturer/importer/distributor, who makes] a substantial modification of [a software product] shall be considered a manufacturer"
- many ([Python Software Foundation](https://pyfound.blogspot.com/2023/04/the-eus-proposed-cra-law-may-have.html), [Eclipse Foundation](https://eclipse-foundation.blog/2023/02/23/cyber-resilience-act-good-intentions-and-unintended-consequences), [NLnet Labs](https://blog.nlnetlabs.nl/open-source-software-vs-the-cyber-resilience-act)) believe the broad wording may cause unintentional harm
  + Article 16 implies FOSS devs "might bear legal and financial responsibility for the way their components are applied in someone else's commercial product"
  + instead, "increased liability should be carefully assigned to the entity that has entered into an agreement with the consumer"
  + indirect monetisation (e.g. advertising paid courses & conference tickets) should not always make software qualify as "commercial"
- however scope of any FOSS exemptions should be carefully limited to prevent commercial abuse/loopholes

## personal opinions

- if you hire an engineer to build a safe and they use substandard components, you sue the engineer. The engineer in turn can sue the component makers *if* they had a contract. You don't sure the component makers directly
- I'm sceptical that any new law could realistically override the "PROVIDED AS IS/NO WARRANTY" clause in FOSS licences
  + the lack of warranties for widely-used FOSS libraries is a [problem]({% post_url 2022-07-24-linux-foss-warranty %}) which can & should be [tackled]({% post_url 2023-04-18-os-is-bad %}) separately (and more urgently than the mere commercial libraries which the CRA & PLA target)
- more counterarguments: [OS is Illegal]({% post_url 2023-07-13-os-is-illegal %})
