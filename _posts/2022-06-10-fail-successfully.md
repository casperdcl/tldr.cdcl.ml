---
title: Making errors helpful
src: https://future.com/negative-engineering-and-the-art-of-failing-successfully
categories: [Programming, Communication]
tags: [principles]
---

Pay attention to error verbosity & handling; your future self will thank you for it.

- fail noisily and informatively
- mission-critical killed process not reporting (error) logs? Hard to manage every failure edge case, especially from external sources? Solution: check for "absence of expected completion" rather than "wait for observable failure."
- try to contain (rather than solve) problems
- in production, 85% of time is spent on error handling, issue reporting & triaging (only 15% of time is spent on code)
  + reducing debugging time by 5% is far more valuable than reducing model dev time by 5%
