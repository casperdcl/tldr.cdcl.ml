---
title: Documenting Software Architecture
src: https://arc42.org/overview
categories: [Communication, Programming]
tags: [opinionated, principles, extra-long]
---

What & How: practical, pragmatic approach to documenting architecture.

1. **Intro & Goals**
   1. motivation/business problems solved, e.g. tabulated use cases
   2. 3~5 "quality goals" e.g. reliability/security/maintainability/performance/compatibility
   3. stakeholders (target audience/users)
2. **Constraints**: inappropriate use cases, e.g. "unsupported on Windows"
3. **Context & Scope diagram**
   1. business/domain perspective: diagrams showing relation to other tools/systems
   2. (optional) technical perspective: {% glossary UML %}
4. **Solution Strategy**: tech stack, design pattern
5. **Code (architecture "building blocks") Diagrams**
   1. whitebox: overall API
   2. blackboxes: subcomponents
6. **Runtime Diagram**: list of steps, flowchart, [sequence diagram](https://en.wikipedia.org/wiki/Sequence_diagram)
7. **Deployment Diagram**
   1. hardware/infrastructure requirements
   2. mapping of software building blocks to said hardware
8. **Pervading Ethos**: design patterns, {% glossary UX %} choices, approach to security, "under-the-hood" concepts
9. **Architecture Decisions**: rationale for not doing things differently, e.g. {% glossary ADR %} (worth its own {% glossary TL;DR %} :scroll:)
   - :thinking: personal opinion: ADR seems an {% glossary XY problem %}. The motivation for ADR (i.e. not just *knowing* the decision -- reading source code -- but remembering *motivation* behind it) can be easily be addressed by inline code comments with URLs (e.g. linking to a GitHub comment) and/or commit messages. The only real value of ADR is collating such comments.
10. **Detailed Quality Goals**
    1. more detailed than (1.2) above, e.g. [ATAM "quality attribute utility tree"](https://en.wikipedia.org/wiki/Architecture_tradeoff_analysis_method)
    2. [usage scenarios](<https://en.wikipedia.org/wiki/Scenario_(computing)>), e.g. "processes user input within 1 second" (not to be confused with [use cases](https://en.wikipedia.org/wiki/Use_case))
11. **Risks & Tech Debt**: current issues & tips to manage/reduce/avoid them
12. **Glossary**: domain/technical terms; avoid synonyms & homonyms to maximise identical understanding
