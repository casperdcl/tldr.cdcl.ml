---
title: Sphinx versus Mkdocs
src: https://github.com/iterative/py-template/issues/19#issuecomment-1140296357
categories: [Programming]
tags: [tools-web, product-research, extra-long]
---

- both `sphinx` & `mkdocs` are mature with nearly identical feature matrices, and we're not considering any other options. However, primary intended use is different:
  + `sphinx` is `rst`-first & config via a `py` file
  + `mkdocs` is `md`-first & config via a `yml` file
- IMO because `md` is more widely adopted outside the Python world and is less `html`-code-like (i.e. ironically more Pythonically zen), it's more actively developed.
  + I switched projects I maintain from `sphinx` to `mkdocs` due to nicer themes, extensions & less boilerplate code
  + Also note PyPI [Topic :: Documentation :: Sphinx](https://pypi.org/search/?q=&o=&c=Topic+%3A%3A+Documentation+%3A%3A+Sphinx) has 465 entries, while [Topic :: Documentation](https://pypi.org/search/?q=&o=&c=Topic+%3A%3A+Documentation) has 2051 (implying circa 3x more non-sphinx Python docs projects).

Compare:

## mkdocs

- plugins/extensions/themes
  - <https://github.com/facelessuser/pymdown-extensions> <- ~25 extensions
  - <https://squidfunk.github.io/mkdocs-material> <- theme + ~15 feature categories, Free + $10/month versions
  - <https://github.com/mkdocs/mkdocs/wiki/MkDocs-Plugins> <- ~150 projects
- complexity
  + <https://github.com/iterative/shtab/blob/master/docs/pydoc-markdown.yml>
  + inline extension directives ([`=== tab`, `!!! tip`](https://raw.githubusercontent.com/iterative/shtab/master/docs/use.md))
- example result
  + <https://docs.iterative.ai/shtab>

## sphinx

- plugins/extensions/themes
  - <https://www.sphinx-doc.org/en/master/usage/extensions> <- short builtin list
  - <https://github.com/sphinx-contrib> <- ~100 repos
  - <https://github.com/yoloseem/awesome-sphinxdoc> <- last update >1 year ago, ~65 entries
  - [Framework :: Sphinx](https://pypi.org/search/?c=Framework+%3A%3A+Sphinx) <- 118 projects
- complexity
  + <https://github.com/iterative/PyDrive2/blob/master/docs/conf.py>
  + inline rst directives (e.g. [`.. toctree:: :maxdepth: 2 <list of pages>`](https://raw.githubusercontent.com/iterative/PyDrive2/master/docs/index.rst))
- example result
  + <https://docs.iterative.ai/PyDrive2>