---
title: Deno JS runtime advantages
src: https://matklad.github.io/2023/02/12/a-love-letter-to-deno.html
categories: [Programming]
tags: [opinionated, oss, principles]
---

New JavaScript runtime ([`deno`](https://github.com/denoland/deno)) tries to fight the "worse-is-better law of software evolution".

- simplifies software development by removing "accidental complexity"
  + e.g. implicit dependencies, environment requirements, abstraction layers (docker)
- builtin formatter (`deno fmt`), LSP server (`deno lsp`), deployment packager (`deno vendor`), transpilation-free TypeScript runtime (`deno main.ts`)
- no reliance on system shell, instead provides [`deno_task_shell`](https://github.com/denoland/deno_task_shell)
  + avoids compatibility issues between `(b?a|z|t?c)sh`
  + `Makefile`-like entrypoints without relying on `make` nor system shell
- some builtin safety, e.g. `deno run https://shady.website/main.ts < in.txt` can only read the explicitly specified input
- no package registry nor manager, instead lockfiles use URLs (optionally can self-host registries)
  + (personal opinion: the public will create a de-facto global registry)
- provides "stable" runtime APIs for unified cross-platform interface
- stdlib is separate (like any dependency) from base `deno` binary
  + ongoing effort for more batteries-included stdlib
- :crossed_swords: con: only runs TypeScript and/or JavaScript (rather than a sane language)
