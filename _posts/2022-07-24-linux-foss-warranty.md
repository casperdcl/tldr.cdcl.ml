---
title: Policing FOSS
src: https://www.technologyreview.com/2022/07/14/1055894/us-military-sofware-linux-kernel-open-source
categories: [Programming, Industry, Law]
tags: [opinionated, principles, oss, ai, law, security]
---

Is it feasible to provide a warranty for {% glossary FOSS %} like the Linux kernel and Python?

- the world's servers rely on the [Linux kernel](https://github.com/torvalds/linux)
  + it's open source and not policed
  + kernel security isn't well understood
  + has contributors from China and Russia, so "the [US] government is [aware that] critical infrastructure [code] could be [...] written by sanctioned entities"
- even proprietary software might be >70% built on {% glossary OSS %}
- the US military wants to prevent [crackers](https://en.wikipedia.org/wiki/Software_cracking) from injecting malicious code into FOSS
- currently, the FOSS world is largely self-regulating and manually tracks security threats
- [DARPA's SocialCyber](https://www.darpa.mil/program/hybrid-ai-to-protect-integrity-of-open-source-code) project will use {% glossary AI %} to detect FOSS threats
  + malicious code, poor code, under-maintained projects & unhealthy dev communities
  + focus on e.g. Linux kernel, Python, etc.
- FOSS contributors' "identities [...] are often obscure, making it hard to hold them accountable"
  + :stop_sign: (personal opinion) FOSS licences tend to explicitly state "provided as-is, no warranty." (Interestingly, the [GPL-2.0](https://opensource.org/licenses/GPL-2.0), which covers the Linux kernel, goes further to allow optional warranties for a fee.) So while it's fine to detect & delete bad code, and even kickban malicious people from FOSS projects, it's probably not possible to hold said people legally accountable
  + :sweat_smile: (personal opinion) there's a more legally sound albeit probably less feasible solution. Does DARPA intend to review the Linux kernel in detail and provide its own warranty? Would that mean I could sue DARPA the next time my {% glossary OS %} crashed?
