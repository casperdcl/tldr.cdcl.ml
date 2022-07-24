---
title: Email breach via expiring domain takeover
src: https://python-security.readthedocs.io/pypi-vuln/index-2022-05-24-ctx-domain-takeover.html
src_suffix: '?utm_source=tldr.cdcl.ml'
categories: [Programming]
tags: [tools-web, security]
---

Don't let your domains expire, or don't use them for email.

- someone took over an expiring domain to get a dev's emails
- no 2FA so could use email to reset passwords & upload to [PyPI](https://pypi.org)
- original dev appears inactive

why it's not too bad (in this particular case):

- compromised package is not really used (few thousand mirror downloads but no obvious libs depend on it)
