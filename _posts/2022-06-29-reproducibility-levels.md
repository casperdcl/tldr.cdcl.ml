---
title: '8 Levels of Reproducibility'
categories: [Programming]
tags: [opinionated, principles, security]
---

> Source: <https://www.anaconda.com/blog/8-levels-of-reproducibility>. I'm happy being at "level 5 reproducibility" for most [FOSS](https://en.wikipedia.org/wiki/Free_and_open-source_software) projects. What concerns me more is [APIs are forever]({% post_url 2022-06-23-apis-are-forever %}).

- -1: not reproducible
- 0: reproducible only by you, today
- 1: reproducible by others, with your guidance
- 2: reproducible by others, today
- 3: reproducible by others
- 4: reproducible by others, without internet access (package all deps into one binary so no reliance on `pip`/`conda` repos)
  + personally I question this. There's no problem relying on `tqdm==4.64.0` being always available on PyPI servers IMO. I'd prefer defining "level 4" as "no need to read installation instructions -- it's obvious just `pip install thing[all]` is needed". AFAIK truly packaging all deps into one binary is level 5 (below)
- 5: reproducible with Docker
- 6: reproducible with a VM (wrapping Docker in a VM)
  + I'd question the value-added of this wrapping
- 7: reproducible on untouched hardware (VM on air-gapped physical hardware kept physically locked)
  + preparing for armageddon, are we?