---
title: Best practice API design
src: https://thenewstack.io/werner-vogels-6-rules-for-good-api-design
categories: [Programming]
tags: [principles]
---

From [AWS](https://aws.amazon.com) CTO.

- **APIs are Forever**: never delete or change an API, otherwise you will break the businesses that build on top of it
- **Never Break Backward Compatibility**: Modifications/improvements are fine but shouldn't break legacy calls the API
- **Work Backwards from Customer Use Cases**: DO NOT design API starting with what the engineers think is good. Instead, work backwards from user's use cases and make a minimal viable API. Simplicity is a feature - it makes it easy to build on top of (both library code & user code)
- **Self-Describing & Clear, Specific Purpose**: thorough up-to-date docs are NOT enough. APIs themselves should also be intuitive at first glance
- **Explicit & Well-Documented Failure Modes**: faulty input parameters, security considerations - not just what your API does, but also how it fails
- **Avoid Leaking Implementation Details at All Costs**: underlying implementation details should not become part of the API itself lest customers build on top to rely on these non-essential details