---
title: Best dev practices from experience
src: https://grugbrain.dev
categories: [Programming]
tags: [opinionated, principles, extra-long]
---

Excellent content written in the worst possible way. The deliberately bad language is fun for a few sentences, but quickly becomes painfully obfuscating. Ironic for something that advocates reduced complexity.

- avoid complex implementations (because they are unmaintainable)
  + if unavoidable (due to business requirements), then try to be as minimal as possible - only make an {% glossary MVP %} or even [just 80% of an MVP](https://en.wikipedia.org/wiki/Pareto_principle)
- readability/maintainability is far more important than {% glossary DRY %}, and more important than "does it work" (!) (if others can understand it they can fix it)
- don't obsess over layout/(re)factoring too early in a project, otherwise you may pick an inappropriate layout which will harm long-term development
- when more mature, try to keep refactoring PRs small & incremental
- don't overdo closures
- don't prematurely optimise
- simpler is better for concurrency models (e.g. stateless request handlers & job queues with no inter-dependencies)
  + use the occasional [thread local var](https://en.wikipedia.org/wiki/Thread-local_storage) if needed
- if you're exploring/prototyping (i.e. don't yet fully understand the problem/use case) then avoid test-driven-development
- write tests after prototyping
- [unit tests](https://en.wikipedia.org/wiki/Unit_testing) often too tiny, [e2e testing](https://smartbear.com/solutions/end-to-end-testing) often too vague/big/flaky. Try in-between ([integration](https://en.wikipedia.org/wiki/Integration_testing)) tests instead, i.e. test interfaces between units
- avoid [mocking](https://en.wikipedia.org/wiki/Mock_object)
- when a bug is reported, write a test for it before fixing it
- don't be over-zealous about dev processes (agile isn't always perfect)
- don't delete code you don't understand. Understand it, decide it's bad, then delete
- master debugging tools
- (:warning: random opinion) typing is mostly about helping autocompletion than helping guarantee correctness
- (:warning: loaded opinion, worth its own {% glossary TL;DR %}) [SoC](https://en.wikipedia.org/wiki/Separation_of_concerns) might miss the point, [LoB](https://htmx.org/essays/locality-of-behaviour) might be better
- (:warning: loaded opinion) the [visitor pattern](https://en.wikipedia.org/wiki/Visitor_pattern) is bad
- (:warning: loaded opinion) splitting dev into {% glossary FE %} and {% glossary BE %} causes unnecessary duplication of efforts
- log a lot, especially for cloud apps
  + major logic branches (if/for)
  + request IDs (to trace across a network)
  + ideally dynamically controlled verbosity
  + ideally per-user controlled verbosity
- design APIs thinking of their use (rather than implementation/domain). {% glossary KISS %} and remember the {% glossary MVP %}
- be sceptical of an revolutionary idea. It's probably been tried before & failed
- better to ask for help than live in FOLD (fear of looking dumb)/impostor syndrome
