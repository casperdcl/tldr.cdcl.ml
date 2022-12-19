---
title: 'Build for "real" developers'
src: https://future.com/software-development-building-for-99-developers
categories: [Programming]
tags: [principles, agile]
---

Putting the majority (but not all) of future maintainers & consumers first.

- build for "real" devs (99%: insurance, healthcare, retail, banking) rather than influencer-hyped-up edge cases (1%: big-tech unicorns)
- large-scale solutions don't work for medium-sized problems
- best engineering practices constantly change; there's no fixed gold standard. Instead, teams should constantly iterate on defining processes
- for users, "progress/good-enough/fit-for-purpose" is the goal, not "pristine code/100% reliability/perfect security" beyond realistic requirements. [You don't need 100% code coverage](https://testing.googleblog.com/2020/08/code-coverage-best-practices.html) - 90% is likely more than enough, make sure you also (*cough*) [test in prod](https://increment.com/testing/i-test-in-production) to "test systems rather than just code"
  + to be able to test-in-production, errors must be both non-silent actually useful/informative
- true value of a product doesn't fit in a 1-min demo/GIF. Needs to stand up on "day 2" too:
  + {% glossary e2e %} test-run things properly
  + integrate with existing workflows
  + reduce (collaboration) friction
- migration (replacing systems/workflows) should be continuous/agile. If it's discrete/waterfall instead, then it'll be slow & users will have to rely on legacy solutions for longer
