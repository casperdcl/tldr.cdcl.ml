---
title: Programming Principles
src: https://wou.edu/las/cs/csclasses/cs161/Lectures/rulesofthumb.html
src_suffix: '?utm_source=tldr.cdcl.ml'
categories: [Programming, Management]
tags: [opinionated, principles]
---

Maintaining clean code & making realistic dev time estimates.

1. :clamp: {% glossary KISS %}
   - especially subprograms:
     * do ONE task (e.g. either {% glossary I/O %} OR algorithmic logic)
     * code short enough to be easily visually inspectable (circa ONE page)
   - for independently decomposable subproblems: separately implement & test before combining
     * "[A complex system that works is invariably [...] evolved from a simple system. [Conversely,] a complex system designed from scratch never works and cannot be made to work](<https://en.wikipedia.org/wiki/John_Gall_(author)#Gall's_law>)"
2. :repeat_one: code may be duplicated ONCE
   - [anything more warrants abstraction into a separate reusable procedure](https://martinfowler.com/books/refactoring.html)
   - alternative is bad design, bad habit, hard to maintain
3. :hourglass: "small" last-mile problems are often hard
    - [first 90% of code = first 90% of dev time; remaining 10% = the remaining 90% :sweat_smile: of dev time](https://en.wikipedia.org/wiki/Ninety%E2%80%93ninety_rule)
4. :confounded: over-optimisation: never sacrifice clarity for efficiency
   - [profile](https://en.wikipedia.org/wiki/Profiling_(computer_programming)) to find the small bottlenecks of code ([likely ~10%](https://en.wikipedia.org/wiki/Program_optimization#Bottlenecks)) to optimise
5. :label: use naming conventions for identifiers (variables, types, functions)
   - easier to read & understand (and thus maintain) code
   - sane style (e.g. no extra-long names nor unclear abbrev.)
   - holy wars over what style to pick are not important; just pick one consistently
   - tips:
     * descriptive of contents
     * or common lang-specific practice (e.g. `i, j, k` for indices)
     * subprogram names: use verb phrases; i.e. ONE -- see rule (1) above -- activity description
     * variable names: nouns (things) or adjectives (attributes)
     * difficulty finding a name indicates code needs refactoring, better design, clarification of purpose of subprograms/variables
